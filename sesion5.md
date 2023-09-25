<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

Ejercicios - while

1.	Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner Ingresar = new Scanner (System.in);
        System.out.println("Introduce un numero");
        int Factor1 = Ingresar.nextInt();
        for (int Factor2=1;Factor2<=10;Factor2++){
            System.out.println(Factor1+"x"+Factor2+"="+ (Factor1*Factor2));
        }
    }
}

2	Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

           System.out.println("Hello World!");
        Scanner sc = new Scanner(System.in);
        System.out.println("Inrese un numero");
        String numero = sc.nextLine();

        int i = 0;
        int contarNumero = 0;

        while (i < numero.length()) {
            char caracter = numero.charAt(i);
            if (caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4' || caracter == '5'
                    || caracter == '6' || caracter == '7' || caracter == '8' || caracter == '9') {
                contarNumero++;
            }
            i++;

        }
        System.out.println("La cadena ingresada contiene:" + contarNumero + "numero");
    }
}

Ejercicios - do while

1	Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

    System.out.println("Hello World!");
        Scanner scanner = new Scanner(System.in);
        System.out.println(" Ingrese el numero");
     int numero;
       int i=0;
       do{
           System.out.println(i+1);
           i++;
           numero = scanner.nextInt();
           if (numero <= 0){
               System.out.println("Numero negativo");
           }
            }
        while (i < 100);
            
    } }

2	Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

System.out.println("Hello World!");
        Scanner Ingresar = new Scanner (System.in);
        System.out.println("Introduce un numero");
        int Factor1 = Ingresar.nextInt();
        
        System.out.println("Introduce un numero");

        if (Factor1 >0){
        for (int Factor2=1;Factor2<=10;Factor2++){
            System.out.println(Factor1+"x"+Factor2+"="+ (Factor1*Factor2));
        }
        }else {
        System.out.println("El numero es 0");
        }
      }
 
 Ejercicios - do while

       1 Imprimir los números impares del 1 al 50.

        System.out.println("Hello World!"); {
        
        int x=0;
        for ( x=0; x<50; x++){
            if ((x%2) !=0){
                System.out.println("El numero es impar"+x);
                
            }
            
        }
    }

    int limite;

        Scanner leer = new Scanner(System.in);
        System.out.println("Ingrese un numero");

        limite = leer.nextInt();

        for (int i = 1; i < limite; i++) {
            int count = 0;

            for (int j = 1; j <= i; j++) {
                if (i % j == 0) {
                    count++;
                }

            }
            if (count == 2) 
            System.out.println(i);
        }


        2.	Imprimir los números primos del 1 al 100.
public class App {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        int limite;

        Scanner leer = new Scanner(System.in);
        System.out.println("Ingrese un numero");

        limite = leer.nextInt();

        for (int i = 1; i < limite; i++) {
            int count = 0;

            for (int j = 1; j <= i; j++) {
                if (i % j == 0) {
                    count++;
                }

            }
            if (count == 2) 
            System.out.println(i);
        }

        
        

    }
}










