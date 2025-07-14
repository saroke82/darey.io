<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Calculator App</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      background-color: #f0f2f5;
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .calculator {
      background-color: #ffffff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.1);
      width: 300px;
    }

    .display {
      width: 100%;
      height: 60px;
      background-color: #222;
      color: #fff;
      font-size: 2rem;
      text-align: right;
      padding: 10px;
      border-radius: 8px;
      margin-bottom: 20px;
      overflow-x: auto;
    }

    .buttons {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
    }

    button {
      font-size: 1.4rem;
      padding: 15px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      background-color: #e0e0e0;
      transition: background-color 0.3s;
    }

    button.operator {
      background-color: #4a90e2;
      color: white;
    }

    button.equal {
      background-color: #00c853;
      color: white;
      grid-column: span 2;
    }

    button.clear {
      background-color: #ff5252;
      color: white;
      grid-column: span 2;
    }

    button:hover {
      background-color: #ccc;
    }

    button.operator:hover {
      background-color: #357ab7;
    }

    button.equal:hover {
      background-color: #00b44b;
    }

    button.clear:hover {
      background-color: #e04646;
    }
  </style>
</head>
<body>

  <div class="calculator">
    <div class="display" id="display">0</div>
    <div class="buttons">
      <!-- Row 1 -->
      <button class="clear" onclick="clearDisplay()">C</button>
      <button class="operator" onclick="appendOperator('/')">÷</button>
      <!-- Row 2 -->
      <button onclick="appendNumber('7')">7</button>
      <button onclick="appendNumber('8')">8</button>
      <button onclick="appendNumber('9')">9</button>
      <button class="operator" onclick="appendOperator('*')">×</button>
      <!-- Row 3 -->
      <button onclick="appendNumber('4')">4</button>
      <button onclick="appendNumber('5')">5</button>
      <button onclick="appendNumber('6')">6</button>
      <button class="operator" onclick="appendOperator('-')">−</button>
      <!-- Row 4 -->
      <button onclick="appendNumber('1')">1</button>
      <button onclick="appendNumber('2')">2</button>
      <button onclick="appendNumber('3')">3</button>
      <button class="operator" onclick="appendOperator('+')">+</button>
      <!-- Row 5 -->
      <button onclick="appendNumber('0')">0</button>
      <button onclick="appendNumber('.')">.</button>
      <button class="equal" onclick="calculateResult()">=</button>
    </div>
  </div>

  <script>
    const display = document.getElementById('display');
    let currentInput = '';
    let resultDisplayed = false;

    function appendNumber(num) {
      if (resultDisplayed) {
        currentInput = '';
        resultDisplayed = false;
      }
      if (currentInput === '0' && num !== '.') {
        currentInput = num;
      } else {
        currentInput += num;
      }
      updateDisplay();
    }

    function appendOperator(op) {
      if (resultDisplayed) {
        resultDisplayed = false;
      }

      if (currentInput === '') return;
      const lastChar = currentInput.slice(-1);
      if ("+-*/".includes(lastChar)) {
        currentInput = currentInput.slice(0, -1);
      }
      currentInput += op;
      updateDisplay();
    }

    function calculateResult() {
      try {
        const result = eval(currentInput);
        currentInput = result.toString();
        resultDisplayed = true;
        updateDisplay();
      } catch (error) {
        display.textContent = 'Error';
      }
    }

    function clearDisplay() {
      currentInput = '';
      resultDisplayed = false;
      updateDisplay();
    }

    function updateDisplay() {
      display.textContent = currentInput || '0';
    }
  </script>

</body>
</html>
