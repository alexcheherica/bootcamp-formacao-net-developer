#  Operadores Aritméticos em C#

Este repositório traz exemplos práticos e explicações sobre **Operadores Aritméticos em C#**, abordando desde conceitos básicos até o uso da classe `Math` para cálculos mais avançados.  


---

##  Introdução aos Operadores Aritméticos

Os operadores aritméticos em C# são usados para realizar operações matemáticas básicas.  

- `+` (Adição)  
- `-` (Subtração)  
- `*` (Multiplicação)  
- `/` (Divisão)  
- `%` (Módulo - resto da divisão)  

 Exemplo:  

```csharp
int a = 10;
int b = 3;

Console.WriteLine(a + b); // 13
Console.WriteLine(a - b); // 7
Console.WriteLine(a * b); // 30
Console.WriteLine(a / b); // 3
Console.WriteLine(a % b); // 1
```
##  Criando a nossa Classe Calculadora

Podemos encapsular as operações em uma classe **Calculadora** para facilitar a reutilização do código.

```csharp
public class Calculadora
{
    public int Somar(int x, int y) => x + y;
    public int Subtrair(int x, int y) => x - y;
    public int Multiplicar(int x, int y) => x * y;
    public double Dividir(double x, double y) => x / y;
}

```
Uso:

```csharp
var calc = new Calculadora();
Console.WriteLine(calc.Somar(5, 7)); // 12

```

## Usando Potência

Para calcular potência, utilizamos o método `Math.Pow(base, expoente)`.

```csharp
double resultado = Math.Pow(2, 3); 
Console.WriteLine(resultado); // 8

```

## Funções Trigonométricas

A classe `Math` também oferece funções trigonométricas:

```csharp
double angulo = Math.PI / 4; // 45 graus

Console.WriteLine(Math.Sin(angulo)); // Seno
Console.WriteLine(Math.Cos(angulo)); // Cosseno
Console.WriteLine(Math.Tan(angulo)); // Tangente

```

## Incremento e Decremento

São operadores que aumentam ou diminuem o valor de uma variável em 1 unidade.

 `++`(incremento)

`--` (decremento)

```csharp
int numero = 5;

numero++;
Console.WriteLine(numero); // 6

numero--;
Console.WriteLine(numero); // 5
```

## Calculando Raiz Quadrada

Para calcular a raiz quadrada, usamos `Math.Sqrt(numero)`.

```csharp
double raiz = Math.Sqrt(25);
Console.WriteLine(raiz); // 5
```

## Conclusão

Com os operadores aritméticos e a classe Math, conseguimos realizar desde operações simples até cálculos mais avançados em C#.
Esse conhecimento é essencial para construir programas que envolvam lógica matemática, jogos, sistemas financeiros e muito mais.

