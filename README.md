# Comissaodovendedor
Comissão para um vendedor de veiculos 

package exercicios;

import java.util.Scanner;

//Uma revendedora de carros usados paga seu funcionario vendedores um salario fixo por mes
//mais uma comissao tambem fiza para cada carro vendido e mais 5% do valor das vendas
//por ele efetuandas Escrever um algoritmo que leia o numero de carros por ele vendidos.
//o valor total de suas vendas o salario fixo e o valor que ele receber por carro vendido
//calcule e escrever o salario final do vendedor


public class Exercicio11 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Salario do funcionario fixo por mes :");
		float salarioFixo = sc.nextFloat();
		
		System.out.println("Valor da comisao que recebe por cada carro vendido : ");
		float qtdCarroVendido = sc.nextFloat();
		
		System.out.println("digite o valor de carros vendidos no mes: ");
		float comissaoFixa = sc.nextFloat();
		
		System.out.println("digite o valor vendido no mes: ");
		float valorTotal = sc.nextFloat();
		
		float totalComissao = qtdCarroVendido*comissaoFixa;
		float porcentagemValor = valorTotal*5/100;
		float valorFinal = salarioFixo+totalComissao+porcentagemValor;
		
		
		System.out.println("O funcionario iria ganhar com comisao : R$" +valorFinal);

	}

}
