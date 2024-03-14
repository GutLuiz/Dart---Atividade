# atividade de Dart

## 1 
```dart
import 'dart:io';

void main() {
  print("Digite a temperatura em Fahrenheit: ");
  double fahrenheit = double.parse(stdin.readLineSync()!);
  double celsius = (fahrenheit - 32) * (5 / 9);
  print("$fahrenheit Fahrenheit = $celsius Celsius");
}
```
## 2
```dart
import 'dart:io';
void main() {
  print("Digite a hora: ");
  int hora = int.parse (stdin.readLineSync()!);
  print("Digite os minutos: ");
  int minutos = int.parse (stdin.readLineSync()!);
  print("Digite os segundos: ");
  int segundos = int.parse (stdin.readLineSync()!);
  int soma = (hora * 3600) + (minutos * 60) + segundos ;
  print("o total de segundos é $soma");
}

```
## 3
```dart
import 'dart:io';
void main() {
  print("digite o custo: ");
  double custo = double.parse (stdin.readLineSync()!);
  print("digite o preço do convite: ");
  double convite = double.parse (stdin.readLineSync()!);
  double conta = custo / convite;
  print("preciso vender pelo menos $conta convites");
}

```
## 4
```dart
import 'dart:io';
void main() {
  print("digite o salario: ");
  double salario = double.parse (stdin.readLineSync()!);
 print("digite o valor das vendas:");
  double vendas = double.parse (stdin.readLineSync()!); 
  double soma = salario + (vendas * 0.12);
  print("o salario final foi $soma");
}

```
## 5
```dart
import 'dart:io';
void main() {
  print("digite o numero de dias de trabalho: ");
  double dias = double.parse (stdin.readLineSync()!);
 double diaria = 38;
 double bruto = dias * diaria;
 double imposto = bruto * 0.06;
 double liquido = bruto  - imposto;
 print("valor da diaria $diaria");
 print("O valor do salario bruto $bruto");
 print("o valor do liquido é $liquido");
print("o valor do imposto é $imposto"); 
}

```
## 6
```dart
import 'dart:io';
void main() {
  print('Digite a duração da chamada em min: ');
  int duracao = int.parse(stdin.readLineSync()!);
  double custo = calcularCustoChamada(duracao);
  print('O total foi de  $custo');
}
double calcularCustoChamada(int duracao) {
  double precoBase = 4.59;
  double custoTotal = precoBase;
  if (duracao > 3) {
    custoTotal += (duracao - 3) * 1.30;
  }
  return custoTotal;
}

```
## 7
```dart
   import 'dart:io';

void main() {
  
     double precoRefrigerante = 8.00;
     double precoSalgado = 12.00;
     double precoSorvete = 9.00;


    stdout.write('Quantidade de refrigerantes: ');
    int Refrigerante = int.parse(stdin.readLineSync()!);

    stdout.write('Quantidade de salgados: ');
    int Salgado = int.parse(stdin.readLineSync()!);

    stdout.write('Quantidade de sorvetes: ');
    int Sorvete = int.parse(stdin.readLineSync()!);

 
    double totalPagar = (Refrigerante * precoRefrigerante) + (Salgado * precoSalgado) +
    (Sorvete * precoSorvete);
       

 
    print('Total a pagar: R\$ ${totalPagar.toStringAsFixed(2)}');
}
```
## 8
```dart
import 'dart:io';


double calcularTotal(int qtdRefrigerante, int qtdSalgado, int qtdSorvete) {
   double precoRefrigerante = 8.00;
   double precoSalgado = 12.00;
   double precoSorvete = 9.00;

  double total = (qtdRefrigerante * precoRefrigerante) +(qtdSalgado * precoSalgado) + (qtdSorvete * precoSorvete);
      (qtdSorvete * precoSorvete);

  return total;
}

double calcularValorPorPessoa(double total, int qtdPessoas) {
  return total / qtdPessoas;
}

void main() {
  stdout.write('Quantidade de refrigerantes: ');
  int qtdRefrigerante = int.parse(stdin.readLineSync()!);

  stdout.write('Quantidade de salgados: ');
  int qtdSalgado = int.parse(stdin.readLineSync()!);

  stdout.write('Quantidade de sorvetes: ');
  int qtdSorvete = int.parse(stdin.readLineSync()!);

  stdout.write('Quantidade de pessoas: ');
  int qtdPessoas = int.parse(stdin.readLineSync()!);

  double total = calcularTotal(qtdRefrigerante, qtdSalgado, qtdSorvete);
  double valorPorPessoa = calcularValorPorPessoa(total, qtdPessoas);

  print('Total a ser pago: R\$ ${total.toStringAsFixed(2)}');
  print('Valor a ser pago por pessoa: R\$ ${valorPorPessoa.toStringAsFixed(2)}');
}

```
## 9
```dart
  import 'dart:io';

void main() {
  double precoCarroPopular = 90.00;
  double precoCarroLuxo = 150.00;

  stdout.write('Tipo de carro (popular ou luxo): ');
  String Carro = stdin.readLineSync()!.toLowerCase();

  stdout.write('Quantos dias de aluguel: ');
  int diasAluguel = int.parse(stdin.readLineSync()!);

  stdout.write('Quantos quilômetros foram percorridos: ');
  int kmPercorrido = int.parse(stdin.readLineSync()!);

  double precoTotal = 0.0;

  if (Carro == 'popular') {
    precoTotal += precoCarroPopular * diasAluguel;
    if (kmPercorrido <= 100) {
      precoTotal += kmPercorrido * 0.20;
    } else {
      precoTotal += (100 * 0.20) + ((kmPercorrido - 100) * 0.10);
    }
  } else if (Carro == 'luxo') {
    precoTotal += precoCarroLuxo * diasAluguel;
    if (kmPercorrido <= 200) {
      precoTotal += kmPercorrido * 0.30;
    } else {
      precoTotal += (200 * 0.30) + ((kmPercorrido - 200) * 0.25);
    }
  }

  print('O preço a ser pago é R\$ ${precoTotal.toStringAsFixed(2)}');
}

```
