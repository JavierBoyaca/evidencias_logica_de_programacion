<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 
# Ejercicios de Lógica de Programación

<!-- Su documentación aquí -->
## 1. Crear un programa en Java para calcular el interés de un CDT
```
import java.util.Scanner;
import java.text.DecimalFormat;

public class Main {
    public static void main(String[] args) {
        DecimalFormat decimalFormat = new DecimalFormat("#,###");
        Scanner scanner = new Scanner(System.in);

        System.out.println("Bienvenido al calculador de CDT!");

        // Pedir al usuario que ingrese los datos del CDT
        System.out.print("Ingrese el monto del depósito: ");
        double montoDeposito = scanner.nextDouble();

        System.out.print("Ingrese la tasa de interés anual (%): ");
        double tasaInteresAnual = scanner.nextDouble();

        System.out.print("Ingrese el plazo en meses: ");
        int plazoMeses = scanner.nextInt();

        // Calcular el interés y el monto total al vencimiento
        double tasaInteresMensual = tasaInteresAnual / 12 / 100;
        double interesMensual = montoDeposito * tasaInteresMensual;
        double montoTotalVencimiento = montoDeposito + (interesMensual * plazoMeses);

        // Mostrar el resumen del CDT
        System.out.println("Resumen del CDT:");
        System.out.println("- Monto del depósito: $" + decimalFormat.format(montoDeposito));
        System.out.println("- Tasa de interés anual: " + tasaInteresAnual + "%");
        System.out.println("- Plazo en meses: " + plazoMeses);
        System.out.println("- Interés mensual: $" + interesMensual);
        System.out.println("- Monto total al vencimiento: $" + decimalFormat.format(montoTotalVencimiento));
    }
}
```
_En este algoritmo para calcular un CDT se le pide al usuario que ingrese la información para calcular el CDT por medio de un Scanner para que se solicite ingresar datos a la consola, tales como el monto, la tasa de interés y el plazo en meses.
Luego declarando 3 (double) se divide la tasa de interés anual por la cantidad de meses del año en el primer double. En el segundo para calcular el interés mensual se multiplica el monto del depósito por la tasa de interés mensual y en el último double para calcular el monto total se suma el monto del depósito con la multiplicación del interés mensual por el plazo en meses.
Por último, se le pide a la consola que imprima los resultados basándose en la información ingresada por el usuario. Para ello se declara un System.out.prinln para imprimir los resultados basados  en lo que se declaró en el (double)_

## 2.Calcular la cantidad de materiales necesarios para construir una pared de ladrillos

```
import java.util.Scanner;

public class CantidadLadrillos {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo;
      
      // Solicita las dimensiones de la pared
      System.out.print("Ingrese el largo de la pared en metros: ");
      largo = input.nextDouble();
      System.out.print("Ingrese el alto de la pared en metros: ");
      alto = input.nextDouble();
      System.out.print("Ingrese el ancho de la pared en metros: ");
      ancho = input.nextDouble();

      // Solicita las dimensiones del ladrillo
      System.out.print("Ingrese el largo del ladrillo en metros: ");
      largoLadrillo = input.nextDouble();
      System.out.print("Ingrese el alto del ladrillo en metros: ");
      altoLadrillo = input.nextDouble();
      System.out.print("Ingrese el ancho del ladrillo en metros: ");
      anchoLadrillo = input.nextDouble();

      // Calcula el área de la pared y del ladrillo
      areaPared = largo * alto;
      double areaLadrillo = largoLadrillo * altoLadrillo;

      // Calcula la cantidad de ladrillos necesarios
      cantidadLadrillos = Math.ceil(areaPared / (areaLadrillo * ancho / anchoLadrillo));

      // Muestra el resultado en la consola
      System.out.printf("Para construir la pared se necesitan %.0f ladrillos.", cantidadLadrillos);
   }
}
```

_Primero se debe declarar las variables que se van a tener en cuenta para saber la cantidad de ladrillos que se van a usar para una pared usando double = largo, alto, ancho, areaPared, cantidadLadrillos, largoLadrillo, altoLadrillo, anchoLadrillo.Luego declarando un Scanner se le solicita al usuario que ingrese Ingrese el largo del ladrillo en metros, el alto del ladrillo en metros y el ancho del ladrillo en metros. Luego de solicitar el usuario que ingrese la información simplemente se declaran tres algoritmos , uno que multiplique el largo por el alto para calcular el área de la pared, luego para calcular la cantidad de ladrillos se multiplica él are del ladrillo por el alto de la pared y se divide por el ancho. Luego por consola se imprime el resultado basado en la información agregada por el usuario._





