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

## Aula 02

- `namespace` 
  - Organiza classes
  - Elementos e afins... por pastas
- ``args`` 
  - Array que recebe argumentos de entradas strings
- Diferença entre ***Write*** e ***WriteLine*** 
  - É que o último quebra a linha para debaixo (tipo dá um enter)

```cs
  using System;

  namespace Aula02
  {
          class Program
      {
          static void Main(string[] args)
          {
              Console.WriteLine("Hello, World!");
              if(args.GetLength(0)>0){
                  Console.Write(args.GetValue(0));
              }
    
          }
      }
  }
```

## Aula 03

### Variáveis

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
      int num=0;
    }
  }
```
🚧 Em Desenvolvimento 📚