

<h1>Calculadora em C# com Windows Forms</h1>

<h2>Funcionalidades</h2>
<p>Desenvolvida em C# utilizando o framework .NET (versão 8) e Windows Forms, esta calculadora proporciona uma experiência de usuário rápida e intuitiva com as seguintes funcionalidades:</p>
<ul>
  <li><strong>➕ Soma:</strong> Realize adições com facilidade.</li>
  <li><strong>➖ Subtração:</strong> Efetue subtrações de maneira simples.</li>
  <li><strong>✖️ Multiplicação:</strong> Faça multiplicações de números de forma rápida.</li>
  <li><strong>➗ Divisão:</strong> Realize divisões com precisão.</li>
  <li><strong>➗ Porcentagem:</strong> Calcule a porcentagem de um valor com facilidade.</li>
  <li><strong>🔄 Apagar:</strong> Limpe os valores inseridos para começar uma nova operação.</li>
  <li><strong>✔️ Gerar Resultado:</strong> Obtenha o resultado da operação com um clique.</li>
</ul>

<h2>Tecnologias Utilizadas</h2>
<table>
  <tr>
    <th>Tecnologia</th>
    <th>Versão</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>C#</td>
    <td>17</td>
    <td>Desenvolvida na linguagem C#, oferecendo uma base sólida e robusta.</td>
  </tr>
  <tr>
    <td>.NET</td>
    <td>4.7.2</td>
    <td>Utilização da versão 8 do framework .NET para aproveitar as últimas melhorias.</td>
  </tr>
  <tr>
    <td>Windows Forms</td>
    <td>12</td>
    <td>Construída com Windows Forms para uma experiência gráfica amigável e intuitiva.</td>
  </tr>
</table>

<h2>Lógica de Operações</h2>
<p>Ao escolher uma operação, a lógica utiliza a variável <code>option</code> para determinar a operação desejada. Exemplo para a soma:</p>
<pre><code>option = "+";
num1 = int.Parse(txtTotal.Text);
txtTotal.Clear();
num2 = int.Parse(txtTotal.Text);

if (option.Equals("+"))
    result = num1 + num2;
// Repita a lógica para as demais operações
</code></pre>

<h2>Lógica de Resultado</h2>
<p>Para gerar o resultado, a lógica limpa as variáveis e exibe o resultado na interface:</p>
<pre><code>txtTotal.Clear();
result = 0;
num1 = 0;
num2 = 0;
</code></pre>

<h2>Operações com Múltiplos Números</h2>
<p>Para operações com mais números, utilize um array para armazenar os números e operadores:</p>
<pre><code>int[] numeros;
string[] operadores; 
int resultado;
int contador = 0;
</code></pre>

