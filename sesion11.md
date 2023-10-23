<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 

# Actividad: Ejercicios de Lógica de Programación
<!-- Su documentación aquí -->

## 1.Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

```
package com.mycompany.sesion11punto1;

import java.util.Random;
import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion11Punto1 {

    public static void main(String[] args) {
        int N, num, count =0;
        N=10;
        int [] a = new int [N];
        Random rd = new Random();
        Scanner leer = new Scanner(System.in);
        
        for (int i = 0;i< N;i++){
        a[i]= rd.nextInt(10-1)+1;
        System.out.println(a[i]);}
        System.out.println("Infrese un nemero entre 1 y 10");
        num=leer.nextInt();
        
        while ((num<1) || (num>10)){
        System.out.println ("Debes ingresar un nemero menor a 10");
        num = leer.nextInt();
       }
        for (int i = 0; i < N; i++){
        if (a[i]== num){
        count++;}
        }
        
        System.out.println("El numero"+num+"se repite"+count+"veces");
    }
}
```
# 2. Desarrollar un algoritmo que realice la conversión de binario a decimal.
```
package com.mycompany.sesion11punto2;

import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion11Punto2 {

    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        //Entrada
        int num, ultimoDigito, c=0, decimal=0;
        System.out.println("Digite un numero binario");
        num= obj.nextInt();
        //Proceso
        while (num!=0){
        ultimoDigito=num%10;
        decimal+=ultimoDigito*Math.pow(2,c);
        c++;
        num/=10;}
        
        System.out.println(decimal);
        
        
    }
}

```




