# VerificaTipoTriangulo

package verificatipotriangulo;
 import java.util.Scanner;

public class VerificaTipoTriangulo {

    
    public static void main(String[] args) {
        
        Scanner Scanner = new Scanner(System.in);
        // solicita ao usuario que insira os tre lados do triangulo
        
        System.out.println("Digite o comprimento do primeiro lado do triangulo:");
        Double lado1= Scanner.nextDouble();
        System.out.println("Digite o comprimento do segundo lado do triangulo:");
        Double lado2= Scanner.nextDouble();
        System.out.println("Digite o comprimento do terceiro lado do triangulo:");
        Double lado3= Scanner.nextDouble();
        // verifica o tipo de triangulo
        if (lado1 == lado2 && lado2 == lado3){
            System.out.println(" o triangulo é equilatero.");
        }else if( lado1 == lado2 || lado1 == lado3 || lado2 == lado3){
            System.out.println("o triangulo é isósceles.");
        }else{
            System.out.println("o triangulo é escaleno.");
      }
        // fecha o Scanner
        Scanner.close();
    }
    
}
