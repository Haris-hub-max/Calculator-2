
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colorful Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" disabled>
        <div class="buttons">
            <button class="number" onclick="addNumber(7)">7</button>
            <button class="number" onclick="addNumber(8)">8</button>
            <button class="number" onclick="addNumber(9)">9</button>
            <button class="operator" onclick="addOperator('/')">/</button>
            <button class="number" onclick="addNumber(4)">4</button>
            <button class="number" onclick="addNumber(5)">5</button>
            <button class="number" onclick="addNumber(6)">6</button>
            <button class="operator" onclick="addOperator('*')">x</button>
            <button class="number" onclick="addNumber(1)">1</button>
            <button class="number" onclick="addNumber(2)">2</button>
            <button class="number" onclick="addNumber(3)">3</button>
            <button class="operator" onclick="addOperator('-')">-</button>
            <button class="number" onclick="addNumber(0)">0</button>
            <button class="operator" onclick="addOperator('+')">+</button>
            <button class="equals" onclick="calculate()">=</button>
            <button class="clear" onclick="clearDisplay()">C</button>
        </div>
    </div>
    <script >let display = document.getElementById('display');
let expression = '';

function addNumber(num) {
    expression += num.toString();
    display.value = expression;
}

function addOperator(operator) {
    expression += operator;
    display.value = expression;
}

function calculate() {
    try {
        let result = eval(expression);
        display.value = result;
        expression = result.toString();
    } catch (error) {
        display.value = 'Error';
        expression = '';
    }
}

function clearDisplay() {
    display.value = '';
    expression = '';
}
</script>
  <style>.calculator {
    width: 300px;
    margin: 50px auto;
    padding: 20px;
    background-color:;
    border: 1px solid #ccc;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

#display {
    width: 100%;
    height: 40px;
    font-size: 24px;
    text-align: right;
    padding: 10px;
    border: none;
    border-radius: 10px;
    background-color:black;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    margin-top: 20px;
}

button {n
    padding: 20px;
    font-size: 18px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
}

.number {
    background-color:white ; /* Light blue */
}

.operator {
    background-color: #ffc107; /* Orange */
}

.equals {
    background-color: #34c759; /* Green */
    
}

.clear {
    background-color: #ff3737; /* Red */
    grid-column: 1/2
}
      #body{
          background-color:black;
        }
</style>
</body>
</html>
