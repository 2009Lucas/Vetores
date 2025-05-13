# Vetores
```java
1. Crie um vetor de 10 elementos inteiros. Leia os valores e exiba quantos deles são maiores que 100.
Scanner ler = new Scanner(System.in);
        int[]v = new int [10];
        int i, cM100 = 0;
        
        for (i = 0; i < v.length; i++) {
            System.out.println("Digite um número");
            v[i] = ler.nextInt();
            
            if (v[i] > 100) {
                cM100++;
                
            }
        }
         System.out.println("O vetor possui " +cM100+ " valores maiores que 100.");
    }
    
}

2. Crie um vetor de 10 elementos inteiros. Exiba a soma de todos os valores armazenados no vetor.
 Scanner ler = new Scanner(System.in);
        int[]v = new int [10];
        int i, cM10 = 0;
        int soma = 0;
        for (i = 0; i < 10; i++) {
            System.out.println("Digite um número");
            v[i] = ler.nextInt();
            
         soma=soma + v[i];
                System.out.println("");
            }
         
        System.out.println("A soma dos vetores é: " +soma);
        }
        
    }

3. Crie um vetor de 10 elementos inteiros. Depois de preenchê-lo, mostre os valores na ordem original e, em seguida, na ordem inversa.
  Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];

        for (int i = 0; i < vetor.length; i++) {
            System.out.print("Digite um número: ");
            vetor[i] = ler.nextInt();
        }

        System.out.println("Os números, na ordem original, são: ");
        for (int i = 0; i < vetor.length; i++) {
            System.out.print(vetor[i] + " ");
        }

        System.out.println("Os números, na ordem inversa, são: ");
        for (int i = vetor.length - 1; i >= 0; i--) {
            System.out.print(vetor[i] + " ");
        }
    }
}

4. Leia um vetor de 10 posições com números inteiros e conte quantos números são negativos.
 Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];
        int numI, numNeg = 0;

        for (int i = 0; i < vetor.length; i++) {
            System.out.println("Digite um número: ");
            vetor[i] = ler.nextInt();

            if (vetor[i] < 0) {
                numNeg++;
            }
            System.out.println("Quantidade de números negativos é: " +numNeg);
        }
    }

}

5. Crie um vetor de 10 elementos inteiros. Multiplique todos os elementos por 2 e mostre o vetor resultante.
  Scanner ler = new Scanner(System.in);
         int vetor[] = new int [10];
         int num;
         
         for (int i = 0; i < vetor.length; i++) {
             System.out.println("Digite um número: ");
             vetor[i] = ler.nextInt();
             
             int numMul = vetor[i] * 2;
             
             System.out.println("Os números, multiplicando por 2 aparecem como: " +numMul);
         }
         
    }
    
}

6. Crie um vetor com 10 números inteiros. Depois de preenchido, substitua todos os números negativos por zero e mostre o vetor final.
 Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];

        for (int i = 0; i < vetor.length; i++) {
            System.out.print("Digite um número: ");
            vetor[i] = ler.nextInt();

            if (vetor[i] < 0) {
                vetor[i] = 0;
            }
        }

        System.out.println("COMPILAÇÃO: ");
        for (int i = 0; i < vetor.length; i++) {
            System.out.print(vetor[i] + " ");
        }

        
    }
}

7. Crie um vetor com 10 elementos inteiros e calcule a média de todos os elementos. Em seguida, mostre quais valores são maiores que a média.
 Scanner ler = new Scanner(System.in);
         int vetor[] = new int [10];
         int soma = 0;
         
         for (int i = 0; i < vetor.length; i++) {
             System.out.println("Digite um número: ");
             vetor[i] = ler.nextInt();
         
             soma += vetor[i];
             int media = (int) soma / vetor.length;
             
             System.out.println("Média dos números: " +media);
         }
              System.out.println("Números maiores que a média: ");
        for (int i = 0; i < vetor.length; i++) {
             int media = 0;
            if (vetor[i] > media) {
                System.out.println(vetor[i]);
             

         }
    }
    
}}

8. Crie um vetor com 10 elementos inteiros e mostre quantas vezes o número 5 aparece no vetor.
 Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];
        int numVet = 0;
        
        for (int i = 0; i < vetor.length; i++) {
            System.out.println("Digite um número: ");
            vetor[i] = ler.nextInt();
            
            if (vetor[i] == 5) {
                numVet++;
                 
            }
           
        }
        System.out.println("O número 5 aparece " +numVet+ " vezes na COMPILAÇÃO.");
    }
    
    
}

9. Crie um vetor de 10 posições com números inteiros. Faça um novo vetor contendo apenas os valores que são múltiplos de 3.
 public static void main(String[] args) {
         Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];
        
       
        for (int i = 0; i < vetor.length; i++) {
            System.out.println("Digite um número: ");
            vetor[i] = ler.nextInt();
        }
        
        ArrayList<Integer> multiplosDeTres = new ArrayList<>();
        
       
        for (int i = 0; i < vetor.length; i++) {
            if (vetor[i] % 3 == 0) {
                multiplosDeTres.add(vetor[i]);
            }
        }
        
        System.out.println("MÚLTIPLOS DE 3 ENCONTRADOS: " );
        multiplosDeTres.forEach((num) -> {
            System.out.println(num);
        });
    }
}

10. Crie dois vetores A e B com 10 números inteiros. Gere um terceiro vetor C contendo o maior valor entre A[i] e B[i] em cada posição.
  Scanner ler = new Scanner(System.in);
        int vetor[] = new int[10];   
        int vetor2[] = new int[10];  
        int vetor3[] = new int[10]; 
        
        System.out.println("Digite os 10 números do vetor A:");
        for (int i = 0; i < vetor.length; i++) {
            System.out.print("A[" + i + "]: ");
            vetor[i] = ler.nextInt();
        }

        System.out.println("Digite os 10 números do vetor B:");
        for (int i = 0; i < vetor2.length; i++) {
            System.out.print("B[" + i + "]: ");
            vetor2[i] = ler.nextInt();
        }

        for (int i = 0; i < vetor3.length; i++) {
            vetor3[i] = Math.max(vetor[i], vetor2[i]);
        }

        System.out.println("Vetor C contém os números: ");
        for (int i = 0; i < vetor3.length; i++) {
            System.out.println("C[" + i + "] = " + vetor3[i]);
        }

    }
}

```
