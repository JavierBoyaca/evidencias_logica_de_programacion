<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 
# En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.

<!-- Su documentación aquí -->

```
import java.util.Arrays;

public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}
```
_En este arrey podemos avidenciar como se genera un array usando las llaves [] y declarando ahi el arrey para general un bloque de numeros. Luego podemos ver como se crea un elemento FOR para calcular la suma de los elemtos del arrey y posteriomente encontrar cual es el numero mas grande dentro del arrey creando un segundo FOR._ 

# Ejemplo Array list
```
import java.util.ArrayList; 
import java.util.Scanner;

public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }

  public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}
```
_En este arreglo podems ver como se hace una lista para pedir al usuruio que ingrese informacion por consola. Por medio de un While pide al usrioa infresar informacion para identificar si es verdadero o falso_

##  Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.
```
package com.mycompany.sesion7;


import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion7 {

    public static void main(String[] args) {
        
        Scanner l = new Scanner(System.in);
         System.out.println("Cuantos candidatos son");
         int candidatos = l.nextInt();
         System.out.println("Cuantos votos hay");
         int votos = l.nextInt();
         int i;
         
         int candidato [] = new int [candidatos];
         int voto []= new int [votos];
         
         System.out.println("Ingrese los voto");
         for (i=0; 1<voto.length;i++){
          voto [i]= l.nextInt();
         }
         for (i=0; i< voto.length; i++){
         candidato[voto[i] = -1]++;
         }
         for (i =0;i< candidato.length;i++){
         System.out.println((i+1)+"-->"+candidato[i]);
         }
            
     }
}
   
```






