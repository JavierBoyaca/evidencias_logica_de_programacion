<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->
1.	Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

        int Numero1 = 10;
        int Numero2 = 20;
        int suma = Numero1 + Numero2;
        int multiplicacion = Numero1 * Numero2;
        System.out.println("el resultado es:" + suma + "\nLa multiplicacion es:" + multiplicacion);

2.	Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números. 

         int Numero1 = 10;
        int Numero2 = 20;
        int resta = Numero1 - Numero2;
        int division = Numero1 / Numero2;
        System.out.println("La resta es:" + resta + "\nLa division es:" + division);

3.	Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

 int Numero1= 30;
 int Numero2 =20;
 int Numero3 = 50;
 int suma = Numero1 + Numero2 + Numero3;
int multiplicacion = Numero1 * Numero2;
int division = Numero1 * Numero2 / Numero3;
 System.out.println("La suma es:" + suma + "\nLa multiplicacion es:"+ multiplicacion + "\nLa division es: "+ division);

4.	Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

double Numero1 = 6.65;
           double Numero2 = 7.85;
                   double suma = Numero1 + Numero2;
        double resta = Numero1 - Numero2;
        double multiplicacion = Numero1 * Numero2;
        double division = Numero1 / Numero2;
 System.out.println("La suma es : " + suma + "\nLa resta es: " + resta +"\nLa multiplicacion es:" + multiplicacion +  "\nLa division es: "+ division);

5.	Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

	int valor = 30;
        valor += 1;
        System.out.println(valor);
        valor -= 1;
        System.out.println(valor);

6.	Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

           int x= 20;
        x += 5 ; 
        System.out.println("x =" + x);
        
7.	Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        Scanner entradaDatos = new Scanner (System.in);
        System.out.println("Infrese le valor boolean");
        boolean valor1 = entradaDatos.hasNextBoolean();
        
        System.out.println("Ingrese el segundo valor boolean");
        boolean valor2 = entradaDatos.hasNextBoolean();
        
        boolean res1 = valor1 && valor2;
        System.out.println("El resultado AND es:");
        System.out.println(res1);
        
        boolean res2 = valor1 || valor2;
        System.out.println("El resultado OR es:");
        System.out.println(res2);
        
        boolean res3 = !valor1;
        System.out.println("El resultado valor 1 negado es:");
        System.out.println(res3);
        
        boolean res4 = !valor1;
        System.out.println("El resultado valor 2 negado es:");
        System.out.println(res4);
        
        
    }
}







