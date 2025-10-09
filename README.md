<!DOCTYPE html>
<html>
<head>
  <title>Simple Calculator</title>
  <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>.calculator {
    width: 300px;
    margin: 50px auto;
    padding: 20px;
    background-color: #f0f0f0;
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
    background-color: #fff;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    margin-top: 20px;
}

button {
    padding: 20px;
    font-size: 18px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
}

.number {
    background-color: #add8e6; /* Light blue */
}

.operator {
    background-color: #ffc107; /* Orange */
}

.equals {
    background-color: #34c759; /* Green */
    grid-column: 2/4;
}

.clear {
    background-color: #ff3737; /* Red */
    grid-column: 1/5;
}
</style>
</head>
<body>
  <div id="calculator">
    <input type="text" id="display" disabled>
    <div>
      <button class="button" onclick="document.getElementById('display').value=''">C</button>
      <button class="button" onclick="document.getElementById('display').value = document.getElementById('display').value.slice(0, -1)">DEL</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '7'">7</button>
      <button class="button" onclick="document.getElementById('display').value += '8'">8</button>
      <button class="button" onclick="document.getElementById('display').value += '9'">9</button>
      <button class="button" onclick="document.getElementById('display').value += '/'">/</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '4'">4</button>
      <button class="button" onclick="document.getElementById('display').value += '5'">5</button>
      <button class="button" onclick="document.getElementById('display').value += '6'">6</button>
      <button class="button" onclick="document.getElementById('display').value += '*'">*</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '1'">1</button>
      <button class="button" onclick="document.getElementById('display').value += '2'">2</button>
      <button class="button" onclick="document.getElementById('display').value += '3'">3</button>
      <button class="button" onclick="document.getElementById('display').value += '-'">-</button>
    </div>
    <div>
      <button class="button" onclick="document.getElementById('display').value += '0'">0</button>
      <button class="button" onclick="document.getElementById('display').value += '.'">.</button>
      <button class="button" onclick="document.getElementById('display').value = eval(document.getElementById('display').value)">=</button>
      <button class="button" onclick="document.getElementById('display').value += '+'">+</button>
    </div>
  </div>
</body>
</html>
