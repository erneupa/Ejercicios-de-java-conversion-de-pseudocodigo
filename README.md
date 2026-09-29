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
Algoritmo contador_impares
	contador<-0
	Mientras contador<=100 Hacer
		Si contador%2<>0 Entonces
			Escribir contador
			contador=contador+1
		SiNo
			contador=contador+1
		Fin Si
	Fin Mientras
FinAlgoritmo

```
![2](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/contador_impares.png)

**3.** Hacer un programa que imprima la suma de los 100 primeros números. 

```
Algoritmo contador_suma
	contador<-0
	Mientras contador<=100 Hacer
		numSuma=numSuma+contador
		contador=contador+1
		Escribir numSuma
	Fin Mientras
FinAlgoritmo
```

![3](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/contador_suma.png)

**4.** Hacer un pseudocódigo que imprima todos los números naturales que hay desde el 0 hasta un número que introducimos por teclado. 
```
Algoritmo imprimir_naturales
	contador<-0
	Escribir "Escribe un numero natural"
	Leer numUsuario
	Mientras contador<=numUsuario Hacer
		Escribir contador
		contador=contador+1
	Fin Mientras
FinAlgoritmo
```

![4](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_naturales.png)

**5.** Introducir un numero por teclado. Que nos diga si es positivo o negativo. 
```
Algoritmo positivo_negativo
	Escribir "Escribe un numero"
	Leer numUsuario
	Si numUsuario<0 Entonces
		Escribir numUsuario, " es negativo"
	SiNo
		Escribir numUsuario, " es positivo"
	Fin Si
FinAlgoritmo

```

![5](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/positivo_negativo.png)

**6.** Programa donde introducimos tantas frases como queramos (el usuario) y contarlas.

```
Algoritmo cadenas_escribir
	seguir=1
	Mientras seguir=1 Hacer
		Escribir "Escribe una frase"
		Leer frase
		
		Escribir "Quieres seguir?? 1(seguir)/2(salir)"
		Leer respuesta
		Si respuesta<>1 Entonces
			seguir=2
			
		SiNo
			seguir=1
		FinSi
	FinMientras
FinAlgoritmo


```
![6](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/cadenas_escribir.png)

**7.** Imprimir y contar los múltiplos de 3 desde 0 hasta un número que introducimos por teclado.

```
Algoritmo multiplos_tres
	Escribir "Escribe un numero"
	Leer numUsuario
	contador<-0
	Mientras  contador<=numUsuario Hacer
		Escribir 3*contador
		contador=contador+1
	Fin Mientras
FinAlgoritmo

```

![7](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/multiplos_tres.png)

**8.** Hacer un pseudocódigo que imprima el mayor y el menor de una serie de cinco números que vamos introduciendo por teclado. 

```
Algoritmo mayor_menor
	contador<-1
	
	
	Mientras contador <= 5 Hacer
        Escribir "Introduce el número ", contador, ":"
        Leer num
        
		Si contador = 1 Entonces
            numMayor <- num
            numMenor <- num
        SiNo
            Si num > numMayor Entonces
                numMayor <- num
            FinSi
            
            Si num < numMenor Entonces
                numMenor <- num
            FinSi
        FinSi
        
        contador <- contador + 1
    FinMientras
    
    Escribir "Mayor: ", numMayor
    Escribir "Menor: ", numMenor
FinAlgoritmo
```

![8](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/mayor_menor.png)

**9.** Introducir dos números por teclado. Imprimir los números naturales que hay entre ambos números empezando por el más pequeño, 
contar cuantos hay y cuantos de ellos son pares. Calcular la suma de los impares.

```
Algoritmo imprimir_entre_pares
	
	Escribir "Escribe el primer número"
	Leer num1
	Escribir "Escribir el segundo número"
	Leer num2
	
	Si num1<num2 Entonces
		numMin<-num1
		numMax<-num2
		
	SiNo
		numMin<-num2
		numMax<-num1
	FinSi
	
	Mientras  numMin<=numMax Hacer
		Escribir numMin
		
		Si numMin%2=0 Entonces
			esPar=esPar+1
			numMin=numMin+1
			
		SiNo
			sumaImpar=sumaImpar+numMin
			numMin=numMin+1
		FinSi
		totalNum=totalNum+1

	
		
		
	Fin Mientras
	
	Escribir "--------------------------------------------------------------------"
	Escribir "Total de números: ",totalNum
	Escribir "Total de números pares: ",esPar
	Escribir "Total suma impares: ",sumaImpar
FinAlgoritmo

```

![9](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_entre_pares.png)


**10.** Imprimir diez veces la serie de números del 1 al 10.
```
Algoritmo imprimir_diez
	contador<-1
	contadorSerie<-1
	
	Mientras contadorSerie<=10 Hacer
		Escribir "Serie ", contadorSerie
		contador<-1
		Mientras contador<=10 Hacer
			Escribir contador
			contador=contador+1
		FinMientras
		contadorSerie=contadorSerie+1
	FinMientras
	
FinAlgoritmo
```

![10](https://github.com/erneupa/PSEUDOC-DIGO-1/blob/main/imprimir_diez.png)


