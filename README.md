# Act_5_Ordenamiento

public class InsertionSort {

    public static void main(String[] args) {

        int[] datos = {905, 210, 550, 102, 443};

        for (int i = 1; i < datos.length; i++) {

            int clave = datos[i];
            int j = i - 1;

            while (j >= 0 && datos[j] > clave) {
                datos[j + 1] = datos[j];
                j--;
            }

            datos[j + 1] = clave;
        }

        System.out.println("Arreglo ordenado:");

        for (int numero : datos) {
            System.out.print(numero + " ");
        }
    }
}
