# Enunciado para exercício inicial sobre Programação Dinâmica

1. Dadas as três versões de implementação de Fibonacci abaixo:
    
    * implemente os algortimos;
    * teste todos para os inteiros 4, 8, 16, 32; 
    * teste os dois últimos também para os inteiro 128, 1000 e 10.000.
    
   ```java
   FIBO-REC (n)
      se n ≤ 1
      então devolva n
      senão a ← FIBO-REC (n − 1)
            b ← FIBO-REC (n − 2)
            devolva a + b
   ```
    
   ```java
   FIBO (n)
    	f [0]  ← 0
	    f [1] ← 1
	    para i ← 2 até n faça
           f[i] <- f[i-1]+f[i-2]
  	  devolva f [n]
   ```
    
   ```java
   int maxVal2(int A[], int init, int end) {  
       if (end - init <= 1)
           return max(A[init], A[end]);  
       else {
             int m = (init + end)/2;
             int v1 = maxVal2(A,init,m);   
             int v2 = maxVal2(A,m+1,end);  
             return max(v1,v2);
            }
   }
   ```
    
2. Monte uma tabela com os resultados das execuções acima. As linhas da tabela são os algoritmos implementados, as colunas os valores para testar e contabilizar.
