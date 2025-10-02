# Tipos de Operadores em C#

##  Operadores de Atribuição

Os operadores de atribuição são usados para **atribuir valores a variáveis**.

* `=` atribui diretamente.
* Também é possível combinar com operações:

  * `+=`, `-=`, `*=`, `/=`, `%=`.

### Conversões de Tipos

* **Convert**: converte valores e trata `null`.
* **Parse**: converte apenas strings válidas.
* **ToString()**: converte para string.
* **Cast implícito**: ocorre quando não há perda de informação.
* **Cast explícito**: precisa ser feito manualmente.
* **Conversão segura**: `TryParse` evita exceções em entradas inválidas.

---

##  Operadores Condicionais

São usados para tomar decisões no fluxo do programa.

* **`if`**: executa um bloco se a condição for verdadeira.
* **`else if` / `else`**: adiciona alternativas.
* **if aninhado**: quando um `if` está dentro de outro.
* **switch case**: simplifica múltiplas verificações de valor.

Exemplo:

```csharp
int x = 10;
if (x > 5)
    Console.WriteLine("Maior que 5");
else
    Console.WriteLine("Menor ou igual a 5");
```

---

##  Operadores Lógicos

Permitem combinar ou inverter condições.

* **OR (`||`)** → verdadeiro se pelo menos uma condição for verdadeira.
* **AND (`&&`)** → verdadeiro apenas se todas as condições forem verdadeiras.
* **NOT (`!`)** → inverte o valor lógico.

Exemplo:

```csharp
bool a = true, b = false;

Console.WriteLine(a || b); // true (OR)
Console.WriteLine(a && b); // false (AND)
Console.WriteLine(!a);     // false (NOT)
```

---

##  Ordem dos Operadores

A ordem de execução segue a **precedência padrão**:

1. Parênteses `()`
2. Operadores unários (`!`, `++`, `--`)
3. Multiplicação, divisão, módulo (`*`, `/`, `%`)
4. Adição e subtração (`+`, `-`)
5. Operadores relacionais (`<`, `>`, `==`, `!=`)
6. Operadores lógicos (`&&`, `||`)
7. Atribuição (`=`, `+=`, `-=` etc.)
