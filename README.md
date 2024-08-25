---
## Desenvolvedor Full-Stack Criativo com Experiência em Aplicações Web e Plataforma de Ensino Interativa"

## Documentação da Calculadora

## Visão Geral

A calculadora **Calc_igor-hilario** é uma aplicação web desenvolvida em HTML, CSS e JavaScript. Ela permite realizar operações matemáticas básicas e avançadas, como adição, subtração, multiplicação, divisão, raiz quadrada e exponenciação. Esta aplicação faz parte de um projeto mais amplo, que inclui também o **Quis**, uma plataforma para questões matemáticas.

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

**Quis** é uma plataforma desenvolvida para a prática e validação de conhecimento matemático por meio de questões de múltipla escolha. A aplicação permite aos usuários responder a perguntas e verificar suas respostas, facilitando o aprendizado e o aprimoramento das habilidades matemáticas.

### Funcionalidades do Quis

- **Questões de Múltipla Escolha**: Usuários podem responder a uma variedade de questões matemáticas.
- **Feedback Imediato**: Respostas corretas e incorretas são informadas imediatamente.
- **Estatísticas de Desempenho**: Acompanhamento do desempenho do usuário com estatísticas e resultados.

### Estrutura HTML do Quis

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Quis - Questões Matemáticas</title>
<style>
/* Estilos CSS aqui */
</style>
</head>
<body>
<div class="quiz-container">
  <header>Quis - Questões Matemáticas</header>
  <div id="question-container">
    <!-- Pergunta será inserida aqui pelo JavaScript -->
  </div>
  <div id="options-container">
    <!-- Opções de resposta serão inseridas aqui pelo JavaScript -->
  </div>
  <button id="next-button" onclick="loadNextQuestion()">Próxima</button>
</div>

<script>
// Código JavaScript aqui
</script>
</body>
</html>
```

### Exemplo de Código JavaScript

```javascript
const questions = [
  {
    question: "Qual é a raiz quadrada de 16?",
    options: ["2", "4", "8", "16"],
    answer: "4"
  },
  {
    question: "Qual é o valor de 5^2?",
    options: ["10", "20", "25", "30"],
    answer: "25"
  }
];

let currentQuestionIndex = 0;

function loadNextQuestion() {
  const questionContainer = document.getElementById('question-container');
  const optionsContainer = document.getElementById('options-container');

  const question = questions[currentQuestionIndex];
  questionContainer.innerHTML = `<p>${question.question}</p>`;
  
  optionsContainer.innerHTML = '';
  question.options.forEach(option => {
    optionsContainer.innerHTML += `<button onclick="checkAnswer('${option}')">${option}</button>`;
  });
}

function checkAnswer(selectedOption) {
  const question = questions[currentQuestionIndex];
  if (selectedOption === question.answer) {
    alert("Resposta Correta!");
  } else {
    alert("Resposta Incorreta. Tente novamente.");
  }
  
  currentQuestionIndex++;
  if (currentQuestionIndex < questions.length) {
    loadNextQuestion();
  } else {
    alert("Quiz concluído!");
  }
}

// Carregar a primeira pergunta ao iniciar
loadNextQuestion();
```

## ODIS (Objetivos de Desenvolvimento e Implementação de Software)

### ODIS do Quis

1. **Objetivo**: Desenvolver uma plataforma interativa para questões matemáticas de múltipla escolha.
2. **Desenvolvimento**: Utilizar HTML, CSS e JavaScript para criar uma interface amigável e funcional.
3. **Implementação**: Garantir que a aplicação seja responsiva e funcione corretamente em diferentes dispositivos e navegadores.
4. **Suporte**: Fornecer documentação e suporte para futuras atualizações e melhorias.

---
