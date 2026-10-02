# Ejercicios-de-java-conversion-de-pseudocodigo

### A continuación, se deben realizar el pseudocódigo y el diagrama de flujo de 
los siguientes enunciados. Se puede utilizar herramientas como PSeInt para 
realizar los ejercicios y verificar el correcto funcionamiento del algoritmo 
planteado. 

**1.** Hacer un pseudocódigo que imprima los números del 100 al 0, en 
orden decreciente. 
```
public class Main {
  public static void main(String[] args) {
    
    int contador = 100;
    
    while (contador>=0) {
        System.out.println(contador);
        contador=contador-1;
    }
    
  }
}

```

![1](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/contador_inverso.png)

**2.** Hacer un pseudocódigo que imprima los números impares entre 0 y 100. 

```
public class Main {
  public static void main(String[] args) {
    
    int contador = 0;
    
    while (contador <=100) {
        if (contador%2==0) {
            System.out.println(contador);
            contador++;
        }
        else {
            contador++;
        }
    }
    
  }
}

```
![2](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/contador_impares.png)

**3.** Hacer un programa que imprima la suma de los 100 primeros números. 

```
public class Main {
  public static void main(String[] args) {
    
    int contador = 0;
    int numSuma = 0;
    
    while (contador <=100) {
       
        contador++;
        numSuma=numSuma+contador;
        System.out.println(numSuma);
        
    }
    
  }
}
```

![3](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/contador_suma.png)

**4.** Hacer un pseudocódigo que imprima todos los números naturales que hay desde el 0 hasta un número que introducimos por teclado. 
```
import java.util.Scanner;
public class main {
	public static void main(String[] args) {
		Scanner escaner = new Scanner(System.in);
		System.out.println("Escribe un número natural");
		
		int numUsuario=escaner.nextInt();
		
		int contador=0;
		
		while (contador<=numUsuario) {
			System.out.println(contador);
			contador++;
		}
	  }
}

```

![4](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_naturales.png)

**5.** Introducir un numero por teclado. Que nos diga si es positivo o negativo. 
```
import java.util.Scanner;
public class main {
	public static void main(String[] args) {
		Scanner escaner = new Scanner(System.in);
		System.out.println("Escribe un número");
		
		int numUsuario=escaner.nextInt();
		
		if (numUsuario<0) {
			System.out.println(numUsuario + " es negativo");
		}
		else {
			System.out.println(numUsuario + " es positivo");
		}
	  }
}

```

![5](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/positivo_negativo.png)

**6.** Programa donde introducimos tantas frases como queramos (el usuario) y contarlas.

```
import java.util.Scanner;
public class main {
	public static void main(String[] args) {
		Scanner escaner = new Scanner(System.in);
		
		
		
		
		int segir=1;
		while (segir==1) {
			
			System.out.println("Escribe una frase");
			String fraseUsuario=escaner.nextLine();
			
			System.out.println("Quieres seguir?? 1(seguir)/2(salir)");
			int respuesta=escaner.nextInt();
			escaner.nextLine();
			
			
			if (respuesta!=1) {
				segir=2;
			}
			else {
				segir=1;
			}
			
		}
	  }
}


```
![6](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/cadenas_escribir.png)

**7.** Imprimir y contar los múltiplos de 3 desde 0 hasta un número que introducimos por teclado.

```

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner escaner=new Scanner(System.in);
        
        System.out.println("Escribe un número");
        int numUsuario = escaner.nextInt();
        
        int contador=0;
        
        while (contador<=numUsuario){
            System.out.println(3*contador);
            contador++;
        }
    }
}

```

![7](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/multiplos_tres.png)

**8.** Hacer un pseudocódigo que imprima el mayor y el menor de una serie de cinco números que vamos introduciendo por teclado. 

```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner escaner=new Scanner(System.in);

        int numUsuario, numMayor = 0, numMenor = 0;
        int contador=1;


        while (contador<=5){
            System.out.println("Escribe el número "+contador+" :");
            numUsuario = escaner.nextInt();

            if (contador==1){
                numMayor=numUsuario;
                numMenor=numUsuario;
            }
            else{
                if (numUsuario > numMayor) {
                    numMayor = numUsuario;
                }

                if (numUsuario < numMenor) {
                        numMenor = numUsuario;
                }
            }
            contador++;
        }

        System.out.println("Mayor: "+ numMayor);
        System.out.println("Menor: "+ numMenor);

    }
}
```

![8](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/mayor_menor.png)

**9.** Introducir dos números por teclado. Imprimir los números naturales que hay entre ambos números empezando por el más pequeño, 
contar cuantos hay y cuantos de ellos son pares. Calcular la suma de los impares.

```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner escaner =  new Scanner(System.in);

        int num1, num2, numMin, numMax, esPar = 0, sumaImpar = 0, totalNum = 0;

        System.out.println("Escribe el primer número:");
        num1=escaner.nextInt();

        System.out.println("Escribe el primer número:");
        num2=escaner.nextInt();

        if (num1<num2){
            numMin=num1;
            numMax=num2;
        }

        else{
            numMin=num2;
            numMax=num1;
        }

        while (numMin<=numMax){
            System.out.println(numMin);

            if (numMin%2==0){
                esPar++;
                numMin++;
            }

            else{
                sumaImpar=sumaImpar+numMin;
                numMin++;
            }

            totalNum++;
        }

        System.out.println("------------------------------------------------");
        System.out.println("Total de números: "+ totalNum);
        System.out.println("Total de números pares: "+ esPar);
        System.out.println("Total suma impares: "+ sumaImpar);
    }
}
```

![9](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_entre_pares.png)


**10.** Imprimir diez veces la serie de números del 1 al 10.
```
public class Main {
    public static void main(String[] args) {

        int contador=1, contadorSerie=1;

        while (contadorSerie<=10){
            System.out.println("Serie " + contadorSerie);
            contador=1;
            while (contador<=10) {
                System.out.println(contador);
                contador++;
            }
            contadorSerie++;
        }
    }
}
```

![10](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_diez.png)


