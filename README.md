# Documentação da Calculadora

## Visão Geral

A calculadora `Calc_igor-hilario` é uma aplicação web simples desenvolvida em HTML, CSS e JavaScript. Ela permite realizar operações matemáticas básicas e avançadas, como adição, subtração, multiplicação, divisão, raiz quadrada e exponenciação.

## Funcionalidades

- **Operações Básicas:** Adição, subtração, multiplicação e divisão.
- **Funções Avançadas:** Raiz quadrada e exponenciação.
- **Interface Limpa e Intuitiva:** Com botões dispostos de forma organizada e um display para mostrar os resultados.

## Layout e Estilo

O design da calculadora inclui:

- **Fundo Geral da Página:** Preto (`#000`).
- **Fundo da Calculadora:** Grafite (`#333`).
- **Cabeçalho:** Texto branco com o nome da calculadora.
- **Botões:** Preto com texto branco, com alguns botões destacados em laranja e verde.

### Estrutura HTML

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Calc_igor-hilario</title>
<style>
/* Estilos CSS aqui */
</style>
</head>
<body>
<div class="container">
  <header>Calc_igor-hilario</header>
  <input type="text" id="display" value="" readonly>
  <br>
  <button class="button orange" onclick="clearDisplay()">C</button>
  <button class="button orange" onclick="backspace()">←</button>
  <button class="button" onclick="appendOperator('/')">÷</button>
  <button class="button" onclick="appendOperator('*')">x</button>
  <br>
  <button class="button" onclick="appendNumber('7')">7</button>
  <button class="button" onclick="appendNumber('8')">8</button>
  <button class="button" onclick="appendNumber('9')">9</button>
  <button class="button" onclick="appendOperator('-')">-</button>
  <br>
  <button class="button" onclick="appendNumber('4')">4</button>
  <button class="button" onclick="appendNumber('5')">5</button>
  <button class="button" onclick="appendNumber('6')">6</button>
  <button class="button" onclick="appendOperator('+')">+</button>
  <br>
  <button class="button" onclick="appendNumber('1')">1</button>
  <button class="button" onclick="appendNumber('2')">2</button>
  <button class="button" onclick="appendNumber('3')">3</button>
  <button class="button green" onclick="calculate()">=</button>
  <br>
  <button class="button" onclick="appendNumber('0')">0</button>
  <button class="button" onclick="appendNumber('.')">.</button>
  <button class="button" onclick="appendOperator('√')">√</button>
  <button class="button" onclick="appendOperator('^')">^</button>
</div>

<script>
// Código JavaScript aqui
</script>
</body>
</html>
