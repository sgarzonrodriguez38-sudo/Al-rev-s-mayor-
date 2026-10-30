
import java.util.Scanner;

public class AlRevesYMayor {

  public static void main(String[] args) {
        Scanner entrada = new Scanner(System.in);
        int[] numeros = new int[5];

        // Pedir los 5 numeros
  for (int i = 0; i < numeros.length; i++) {
            System.out.print("Ingrese un                               numero: ");
            numeros[i] = entrada.nextInt();
        }

        // Mostrar los numeros al reves
   System.out.println("Numeros al reves:");

   for (int i = numeros.length - 1; i >= 0;                                    i--) {
            System.out.print(numeros[i] + "                                        ");
        }

    // Buscar el numero mayor
  int mayor = buscarMayor(numeros);

   System.out.println();
   System.out.println("El mayor es: " +            mayor);
    }

  public static int buscarMayor(int[] numeros) {

   int mayor = numeros[0];

 for (int i = 1; i < numeros.length; i++) {

   if (numeros[i] > mayor) {
                mayor = numeros[i];
            }
        }
      return mayor;
    }
}
