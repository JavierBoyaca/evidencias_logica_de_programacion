<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 
# Implementar los siguientes métodos:

<!-- Su documentación aquí -->
## 1.Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

```
package com.mycompany.actividadsesion8;

import java.util.Scanner;

/**import java.until.*;
 *
 * @author javie
 */
public class ActividadSesion8 {

    public static void main(String[] args) {
        int num1,num2 ;
        Scanner n=new Scanner (System.in);
        System.out.print("Ingrese el primer numero:");
        num1=n.nextInt();
        System.out.print ("Ingrese el segundo numero :");
        num2=n.nextInt();
        
        if (num1>num2){
            System.out.println(num1+"es mayor que"+num2);
        }
        else{
            System.out.println(num2+"es mayor que"+num1);
        }
        
    }
}
```

## 2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

```
package com.mycompany.sesion8punto2;

import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion8Punto2 {

    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
        String cadena;
        int count = 0,i;
        char letra;
        System.out.println("Ingrese una frase:");
        cadena = leer.nextLine();
        
        for (i=0;i<cadena.length();i++){
        letra = Character.toLowerCase(cadena.charAt(i));
        if (letra == 'a' || letra == 'e' || letra == 'i' || letra == 'o' ||letra == 'u' ){
            count++;
        }
        
        
    } 
        System.out.println("La cantidad de vocales son" + count);
    }
}

```

## 3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

```
package com.mycompany.sesion8punto3;

import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion8Punto3 {

    public static void main(String[] args) {
        String palabra="palabra";
        Scanner PL=new Scanner (System.in);
        System.out.println("Ingrese una palabra");
        palabra=PL.nextLine();
        System.out.println(palabra.toUpperCase());
        System.out.println(palabra.toLowerCase());
    }
}
```
## 4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene

```
package com.mycompany.sesion8punto4;

import java.util.Scanner;

/**
 *
 * @author javie
 */
public class Sesion8punto4 {

    public static void main(String[] args) {
        Scanner teclado = new Scanner (System.in);
        System.out.print (" Introduce una cadena de texto: ");
        String cadenaUsuario = teclado.nextLine();
        System.out.println("\nLa cadena tiene" + cuentaPalabras(cadenaUsuario) + "palabras");
        
    }
    public static int cuentaPalabras (String cadena){
    String[]palabras = cadena.trim().split(" +");
    return palabras.length;
    }
}

```








