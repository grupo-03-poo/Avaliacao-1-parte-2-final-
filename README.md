# Avaliação 1 - parte 2 (final)

using System;



namespace Av1_Pt2
{
class Program
{
static void Main(string[] args)
{
//Menu de opções



Console.WriteLine("Escolha uma opção: ");
Console.WriteLine("");



Console.WriteLine("1° - Soma de dois números;");
Console.WriteLine("2° - Diferença entre dois números (maior pelo menor);");
Console.WriteLine("3° - Produto entre dois números;");
Console.WriteLine("4° - Divisão entre dois números (o denominador não pode ser zero);");
Console.WriteLine("5° – Raiz quadrada (o número não pode ser menor que zero);");
Console.WriteLine("6° – Elevar um número ao quadrado.");



Console.WriteLine("");



Console.WriteLine("Digite a opção desejada: ");
string op = Console.ReadLine();
int opcao = Convert.ToInt16(op);



//Verificação do menu; cálculo; impressão.



switch (opcao)
{
case 1:



Console.WriteLine("Digite o primeiro número: ");
string numero1 = Console.ReadLine();
int num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
string numero2 = Console.ReadLine();
int num2 = Convert.ToInt16(numero2);



int soma = num1 + num2;
Console.WriteLine("A soma dos dois número é: " + soma);
break;



case 2:



Console.WriteLine("Digite o primeiro número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
numero2 = Console.ReadLine();
num2 = Convert.ToInt16(numero2);
if (num1 >= num2)
{
int diferenca = num1 - num2;
Console.WriteLine("A diferença entre os números é: " + diferenca);
}
else
{
int diferenca = num2 - num1;
Console.WriteLine("A diferença entre os números é: " + diferenca);
}
break;



case 3:



Console.WriteLine("Digite o primeiro número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
numero2 = Console.ReadLine();
num2 = Convert.ToInt16(numero2);



int produto = num1 * num2;
Console.WriteLine("O produto entre os dois números é: " + produto);
break;



case 4:



Console.WriteLine("Digite o numerador: ");
string numero = Console.ReadLine();
double num = Convert.ToDouble(numero);



Console.WriteLine("Digite o denominador: ");
string numero02 = Console.ReadLine();
double num02 = Convert.ToDouble(numero02);



double divisao = num / num02;
divisao = Math.Round(divisao, 2);



while (num02 == 0)
{
Console.WriteLine("O denominador não pode ser igual a zero.");
Console.WriteLine("");



Console.WriteLine("Digite o numerador: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



Console.WriteLine("Digite o denominador: ");
numero02 = Console.ReadLine();
num02 = Convert.ToDouble(numero02);



divisao = num / num02;
divisao = Math.Round(divisao, 2);



}



Console.WriteLine("A divisão é: " + divisao);
break;



case 5:



Console.WriteLine("Digite um número: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



double raiz = Math.Sqrt(num);
raiz = Math.Round(raiz, 2);



while (num <= 0)
{
Console.WriteLine("O número não pode ser menor ou igual a zero.");
Console.WriteLine("");
Console.WriteLine("Digite um número: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



raiz = Math.Sqrt(num);
raiz = Math.Round(raiz, 2);



}



Console.WriteLine("A raíz do número é: " + raiz);



break;



case 6:
Console.WriteLine("Digite um número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



int quadrado = num1 * num1;
Console.WriteLine("O quadrado do número é: " + quadrado);



break;



}

//Verificação de comando incorretos



while (opcao == 0 || opcao >= 7)
{
Console.WriteLine("Opção Inválida!!!");
Console.WriteLine("");



Console.WriteLine("Digite a opção desejada: ");
op = Console.ReadLine();
opcao = Convert.ToInt16(op);



switch (opcao)
{
case 1:



Console.WriteLine("Digite o primeiro número: ");
string numero1 = Console.ReadLine();
int num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
string numero2 = Console.ReadLine();
int num2 = Convert.ToInt16(numero2);



int soma = num1 + num2;
Console.WriteLine("A soma dos dois número é: " + soma);
break;



case 2:



Console.WriteLine("Digite o primeiro número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
numero2 = Console.ReadLine();
num2 = Convert.ToInt16(numero2);
if (num1 >= num2)
{
int diferenca = num1 - num2;
Console.WriteLine("A diferença entre os números é: " + diferenca);
}
else
{
int diferenca = num2 - num1;
Console.WriteLine("A diferença entre os números é: " + diferenca);
}
break;



case 3:



Console.WriteLine("Digite o primeiro número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



Console.WriteLine("Digite o segundo número: ");
numero2 = Console.ReadLine();
num2 = Convert.ToInt16(numero2);



int produto = num1 * num2;
Console.WriteLine("O produto entre os dois números é: " + produto);
break;



case 4:



Console.WriteLine("Digite o numerador: ");
string numero = Console.ReadLine();
double num = Convert.ToDouble(numero);



Console.WriteLine("Digite o denominador: ");
string numero02 = Console.ReadLine();
double num02 = Convert.ToDouble(numero02);



double divisao = num / num02;
divisao = Math.Round(divisao, 2);



while (num02 == 0)
{
Console.WriteLine("O denominador não pode ser igual a zero");
Console.WriteLine("");



Console.WriteLine("Digite o numerador: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



Console.WriteLine("Digite o denominador: ");
numero02 = Console.ReadLine();
num02 = Convert.ToDouble(numero02);



divisao = num / num02;
divisao = Math.Round(divisao, 2);



}



Console.WriteLine("A divisão é: " + divisao);
break;



case 5:



Console.WriteLine("Digite um número: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



double raiz = Math.Sqrt(num);
raiz = Math.Round(raiz, 2);



while (num <= 0)
{
Console.WriteLine("O número não pode ser menor ou igual a zero!!!");
Console.WriteLine("");
Console.WriteLine("Digite um número: ");
numero = Console.ReadLine();
num = Convert.ToDouble(numero);



raiz = Math.Sqrt(num);
raiz = Math.Round(raiz, 2);



}



Console.WriteLine("A raíz do número é: " + raiz);



break;



case 6:
Console.WriteLine("Digite um número: ");
numero1 = Console.ReadLine();
num1 = Convert.ToInt16(numero1);



int quadrado = num1 * num1;
Console.WriteLine("O quadrado do número é: " + quadrado);



break;



}



}



Console.ReadKey();



}



}
}
