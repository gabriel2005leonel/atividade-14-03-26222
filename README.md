import java.util.Scanner;

public class AulaSabado {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        double saldo = 100;
        int opcao = 0;

        while (opcao != 4) {

            System.out.println("\n1 - Ver saldo");
            System.out.println("2 - Depositar");
            System.out.println("3 - Sacar");
            System.out.println("4 - Sair");
            System.out.print("Escolha: ");

            opcao = sc.nextInt();

            if (opcao == 1) {
                System.out.println("Saldo: " + saldo);
            }

            if (opcao == 2) {
                System.out.print("Valor: ");
                double valor = sc.nextDouble();
                saldo = saldo + valor;
            }

            if (opcao == 3) {
                System.out.print("Valor: ");
                double valor = sc.nextDouble();
                saldo = saldo - valor;
            }

            if (opcao == 4) {
                System.out.println("Saindo...");
            }
        }

        sc.close();
    }
}
