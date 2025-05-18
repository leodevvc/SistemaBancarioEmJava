# SistemaBancarioEmJava
package techwavesolucoesdigitais;

import java.util.Scanner;


public class TechWaveSolucoesDigitais {

    
    public static void main(String[] args) {
        // TODO code application logic here
        
         //Essa parte fica exclusiva para o usuario entrar em sua conta
         
        Scanner teclado = new Scanner(System.in);
        System.out.println("OLA USUARIO, BEM VINDO AO NOSSO BANCO FINANCEIRO");
        System.out.println("Digite seu nome: ");
        String nome = teclado.nextLine();
        System.out.println("Ola " + nome + ", digite seu código verificador:");
        int codigo = teclado.nextInt();
        
        //Essa parte fica exclusiva para o usuario escolher oque deseja
        
        System.out.println("BEM VINDO! COMO PODEMOS RESOLVER SEU PROBLEMA?");
       
        int escolha;
          System.out.println("1-VER SALDO");
          System.out.println("2-FAZER DEPOSITO");
          System.out.println("3- FAZER SAQUE");
          System.out.println("4- SAIR/OUTROS");
        escolha = teclado.nextInt();
        double saldo = 50.00;
         switch (escolha) {
             case 1:
                 System.out.println("PREZADO (A)" + nome +  " ,SEU SALDO É R$:" + saldo);
                 break;
                 
             case 2:
                 System.out.println("DIGITE O VALOR DO DEPOSITO:");
                 double deposito = teclado.nextDouble();
        saldo += deposito;
                  System.out.println("DEPOSITO REALIZADO COM SUCESSO SEU NOVO SALDO É " + saldo);
                  break;
             case 3:
                 System.out.println(" QUAL O VALOR PARA SAQUE? ");
                 
             case 4:
                 System.out.println("OBRIGADO POR USAR O BANCO TECHWAVE. ATÉ A PROXIMA!");
                 break;
         }     
                 
         
         
