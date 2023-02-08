# CFB Cursos - C#

## Aula 01

- `Using System;` 
  - Biblioteca básica com comandos de entradas e saídas e afins...
- **Principal** 
  - Nome dado a class ou programa 
- `Main()` 
  - Método Principal dessa class
  - É o ponto de entrada de um aplicativo C#, exceto em Bibliotecas e serviços.
- `static` 
  - Pertence a classe Principal
- `void` 
  - Não gera valor de retorno
- **Método** 
  - É um bloco de código que contém uma série de instruções

```cs
  using System;

  class Principal {
    
    static void Main() {
      Console.Write("Olá Mundo!");
    }
  }

```
---
## Aula 02
- **Instalação .NET**
  - Comando cmd `dotnet new console`
- `string[] args` 
  - Padrão de argumentos de entrada
- `namespace` 
  - Organiza classes
  - Elementos e afins... por pastas
- `args`
  - Array que recebe argumentos de entradas strings
- Diferença entre ***Write*** e ***WriteLine*** 
  - É que o último quebra a linha para debaixo (tipo dá um enter)
- `GetLength(0)` 
  - Esses valores indicam a dimensão da array que você quer obter o comprimento, args. `GetLength(0)` é o mesmo que ***args.Length***, quando aplicado numa array de uma dimensão.

```cs
  using System;

  namespace Aula02
  {
    class Program
    {
      static void Main(string[] args)
      {
        Console.WriteLine("Hello, World!");
        if(args.GetLength(0)>0)
        {
          Console.Write(args.GetValue(0));
        }
    
      }
    }
  }
```
---
## Aula 03

 ## Variáveis

- **Todas as variáveis abaixo são locais ao método** `Main()`
- `Var` 
  - Operador
  - Não é tipada
  - Recebe a tipagem na atribuição
  - Excessão:
    - Ex: `var aux = nome;` O seu valor é capturado da variável `nome `do Tipo String.
  - Não pode ser alterada depois.
- **Variáveis** 
  - Posição reservada na memória RAM. 
  - Armazena dados(informações)
  - Lê e Altera
- **Declaração** 
  - Criar
- **Atribuir** 
  - Adicionar um valor
- **Linguagem Tipada** 
  - Especificar o tipo de dados
- `int`
  - Inteiro 
  - Tipo primitivo
  - Com sinal
  - Recebe valor negativo
  - Tamanho 32 bits de dados
- `byte` 
  - Inteiro
  - Sem sinal
  - Tamanho 8 bits
  - Armazena entre 0 e 255
- `char` 
  - Caracteres
  - Limitador `''` 
  - Armazena 1 caracter ou 1 número
- `float` 
  - Tipo float
  - Primitivo
  - Ex: `5.3f`
  - `f` indica padrão float
- `string` 
  - Tipo referência
  - Conjunto caracteres `char`
  - Limitador `""` 
  - Não é primitiva
  - Armazena texto

```cs
  using System;

  class Aula03{
    static void Main(){
      byte n1=10; // 0 a 255
      int num=0;
      char letras = '8';
      float valor = 5.3f;
      string nome = "Bruno";

      var aux=nome;

      Console.WriteLine("Valor da variável: " + aux + "...");
    }
  }
```
## Múltiplas Variáveis

- É o ato declarar várias variáveis usando uma mesma tipagem.

```cs
  using System;

class Aula03{
  static void Main(){
    int num1, num2, res;

    num1=10;
    num2=2;
    res = num1 * num2;

    Console.WriteLine("A multiplicação de " + num1 + " Com " + num2 + " é igual a: " + res);
  }
}
```
---

## Aula 04
## Escopo de Variáveis

- Escopo global
  - Declarada e válida dentro da `class`
- Escopo Local
  - Declarada e válida somente dentro de um método
    - Ex: `Main()` ou de outro nome definido `teste()`
    - `static`
    - `void` 

```cs
  using System;

  class Aula04 {

    static int num=10; 
    
    static void Main(){
      int num1=0;
      Console.WriteLine(num);
    }
  }
```

🚧 Em Desenvolvimento 📚