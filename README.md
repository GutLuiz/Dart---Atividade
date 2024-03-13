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

```
## 8
```dart

```
## 9
```dart

```
