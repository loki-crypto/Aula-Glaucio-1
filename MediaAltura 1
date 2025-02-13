import java.util.Scanner;

public class  Main3 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int totalHomens = 0;
        int totalMulheres = 0;
        double somaAlturaHomens = 0;
        double maiorAltura = Double.MIN_VALUE;
        double menorAltura = Double.MAX_VALUE;

        for (int i = 1; i <= 15; i++) {
            System.out.println("Pessoa " + i);

            System.out.print("Digite a altura (em metros): ");
            double altura = scanner.nextDouble();

            System.out.print("Digite o gênero (M para masculino, F para feminino): ");
            char genero = scanner.next().charAt(0);

            if (genero == 'M' || genero == 'm') {
                totalHomens++;
                somaAlturaHomens += altura;
            } else if (genero == 'F' || genero == 'f') {
                totalMulheres++;
            }

            if (altura > maiorAltura) {
                maiorAltura = altura;
            }
            if (altura < menorAltura) {
                menorAltura = altura;
            }
        }

        double mediaAlturaHomens = totalHomens > 0 ? somaAlturaHomens / totalHomens : 0;

        System.out.println("\nResultados:");
        System.out.println("Total de homens: " + totalHomens);
        System.out.println("Total de mulheres: " + totalMulheres);
        System.out.println("Média da altura dos homens: " + mediaAlturaHomens + " metros");
        System.out.println("Maior altura do grupo: " + maiorAltura + " metros");
        System.out.println("Menor altura do grupo: " + menorAltura + " metros");

        scanner.close();
    }
}
