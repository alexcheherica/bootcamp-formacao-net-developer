#  Sintaxe e Estrutura de Código em C#

##  Sintaxe e Indentação

C# é uma linguagem de programação fortemente tipada e baseada em blocos.
Usa chaves `{}` para delimitar blocos de código.
A indentação não afeta a execução, mas é essencial para **legibilidade** e **boas práticas**.

---

##  Estrutura de um Projeto

Um projeto C# geralmente contém:

* Arquivo `.csproj` com configurações do projeto.
* Arquivo `Program.cs` com o ponto de entrada (`Main()`).
* Diretórios como `bin/` e `obj/` gerados na compilação.

---

##  O Conceito de Classe

Classes são estruturas que definem objetos e seus comportamentos.

Exemplo:

```csharp
public class Pessoa 
{
    public string Nome;
    public int Idade;
}
```

---

##  Criando e Usando Classes

Você pode instanciar uma classe com `new`:

```csharp
Pessoa p = new Pessoa();
p.Nome = "Alexchê";
p.Idade = 30;
```

---

##  Namespaces

Servem para organizar o código e evitar conflitos de nomes.

Exemplo:

```csharp
namespace MeuProjeto 
{
    class Program 
    {
        // ...
    }
}
```

---

##  Convenções de Escrita

###  Convenções Case

* **PascalCase**: usado para nomes de classes e métodos (`MinhaClasse`, `CalcularTotal`).
* **camelCase**: usado para variáveis e parâmetros (`minhaVariavel`, `valorTotal`).

###  Boas Práticas

* Nome de classe deve ser **substantivo** e **descritivo**.
* Variáveis devem ter **nomes claros e significativos**.
* Evite abreviações obscuras ou nomes genéricos como `x`, `temp`.

---

##  Tipos de Dados em C#

###  Tipos Inteiros

* `int`: número inteiro de 32 bits.
* `long`: inteiro de 64 bits.
* `short`, `byte`: menores variações.

###  Números Decimais

* `float`: precisão simples.
* `double`: precisão dupla.
* `decimal`: usado para cálculos financeiros com alta precisão.

---

##  Declarando Variáveis

```csharp
int idade = 25;
double altura = 1.75;
string nome = "Alexchê";
```

---

## 🔧 Manipulando Variáveis

Você pode alterar valores, fazer operações matemáticas, concatenar strings, etc.

```csharp
idade += 1;
nome = nome + " Silva";
```

---

## 📅 Tipo DateTime

Representa datas e horas.

```csharp
DateTime hoje = DateTime.Now;
DateTime nascimento = new DateTime(1995, 9, 29);
```
