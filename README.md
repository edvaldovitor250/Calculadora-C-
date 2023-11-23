# Calculadora em C# com Windows Forms

## Funcionalidades

Desenvolvida em C# utilizando o framework .NET (versão 8) e Windows Forms, esta calculadora proporciona uma experiência de usuário rápida e intuitiva com as seguintes funcionalidades:

- **Soma:** Realize adições com facilidade.
- **Subtração:** Efetue subtrações de maneira simples.
- **Multiplicação:** Faça multiplicações de números de forma rápida.
- **Divisão:** Realize divisões com precisão.
- **Porcentagem:** Calcule a porcentagem de um valor com facilidade.
- **Apagar:** Limpe os valores inseridos para começar uma nova operação.
- **Gerar Resultado:** Obtenha o resultado da operação com um clique.

## Tecnologias Utilizadas

| Tecnologia        | Versão | Descrição                                              |
|-------------------|--------|--------------------------------------------------------|
| C#                | 17      | Desenvolvida na linguagem C#, oferecendo uma base sólida e robusta. |
| .NET              | 4.7.2      | Utilização da versão 8 do framework .NET para aproveitar as últimas melhorias. |
| Windows Forms     | 12      | Construída com Windows Forms para uma experiência gráfica amigável e intuitiva. |


## Lógica de Operações

Ao escolher uma operação, a lógica utiliza a variável `option` para determinar a operação desejada. Exemplo para a soma:

```csharp
option = "+";
num1 = int.Parse(txtTotal.Text);
txtTotal.Clear();
num2 = int.Parse(txtTotal.Text);

if (option.Equals("+"))
    result = num1 + num2;
// Repita a lógica para as demais operações


```csharp
option = "+";
num1 = int.Parse(txtTotal.Text);
txtTotal.Clear();
num2 = int.Parse(txtTotal.Text);

if (option.Equals("+"))
    result = num1 + num2;
// Repita a lógica para as demais operações


# Lógica de Resultado

Para gerar o resultado, a lógica limpa as variáveis e exibe o resultado na interface:

```csharp
txtTotal.Clear();
result = 0;
num1 = 0;
num2 = 0;

## Operações com Múltiplos Números

Para operações com mais números, utilize um array para armazenar os números e operadores:

```csharp
int[] numeros;
string[] operadores; 
int resultado;
int contador = 0;

