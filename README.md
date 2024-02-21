# ejerciciotema1https:
//github.com/ladamanegra/ejerciciotema1.git
import java.util.Scanner;

public class uno {
    private Scanner teclado;
    private int diasEnUnAno;
    private int horasEnUnDia;
    private int minutosEnUnaHora;
    private int segundosEnUnMinuto;

    public void cargar() {
        teclado = new Scanner(System.in);
        System.out.println("Ingresa los dias en un año");
        diasEnUnAno = teclado.nextInt();
        System.out.println("Ingresa las horas en un dia");
        horasEnUnDia = teclado.nextInt();
        System.out.println("Ingresa los minutos en una hora");
        minutosEnUnaHora = teclado.nextInt();
        System.out.println("Ingresa los segundos en un minuto");
        segundosEnUnMinuto = teclado.nextInt();
    }

    public void retornar() {
        int segundos = diasEnUnAno * horasEnUnDia * minutosEnUnaHora * segundosEnUnMinuto;
        System.out.println("El total de segundos es: " + segundos);
    }

    public static void main(String[] args) {
        uno un = new uno();
        un.cargar();
        un.retornar();
    }
}
