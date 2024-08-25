---
## Projetos de Desenvolvimento de Software

## Documentação da Calculadora

## Visão Geral

A calculadora **Calc_igor-hilario** é uma aplicação web desenvolvida em HTML, CSS e JavaScript. Ela permite realizar operações matemáticas básicas e avançadas, como adição, subtração, multiplicação, divisão, raiz quadrada e exponenciação. Esta aplicação foi criada como parte de um projeto mais amplo, incluindo também o **Quis**, um projeto separado focado em questões matemáticas.

## Funcionalidades

- **Operações Básicas**: Adição, subtração, multiplicação e divisão.
- **Funções Avançadas**: Raiz quadrada e exponenciação.
- **Interface Limpa e Intuitiva**: Com botões dispostos de forma organizada e um display para mostrar os resultados.

## Layout e Estilo

O design da calculadora inclui:

- **Fundo Geral da Página**: Preto (#000).
- **Fundo da Calculadora**: Grafite (#333).
- **Cabeçalho**: Texto branco com o nome da calculadora.
- **Botões**: Preto com texto branco, com alguns botões destacados em laranja e verde.

## Estrutura HTML

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
```

## Código JavaScript

### Funções Básicas

- **`clearDisplay()`**: Limpa o display.
- **`backspace()`**: Remove o último caractere do display.
- **`appendNumber(number)`**: Adiciona um número ao display.
- **`appendOperator(operator)`**: Adiciona um operador ao display.
- **`calculate()`**: Realiza o cálculo com base na expressão no display.

## Projeto Quis

O **Quis** é um projeto separado focado em questões matemáticas. É uma plataforma onde os usuários podem responder a questões matemáticas de múltipla escolha, permitindo a prática e a validação do conhecimento matemático. Mais detalhes sobre o projeto Quis podem ser encontrados em sua própria documentação ou repositório.

## ODIS (Objetivos de Desenvolvimento e Implementação de Software)

### ODIS da Calculadora

1. **Objetivo**: Desenvolver uma aplicação web simples que permita a realização de operações matemáticas básicas e avançadas.
2. **Desenvolvimento**: Utilizar HTML, CSS e JavaScript para criar uma interface intuitiva e funcional.
3. **Implementação**: Garantir que a calculadora seja responsiva e funcione corretamente em diferentes dispositivos e navegadores.
4. **Suporte**: Manter a documentação atualizada e fornecer suporte para futuras atualizações e melhorias.

---

Essa documentação agora inclui uma seção sobre o projeto **Quis** e detalha os **ODIS** relacionados ao desenvolvimento e implementação da calculadora. Se precisar de mais alguma coisa, é só avisar!
