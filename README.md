  <html>
  <head>
      <title>simple calculator</title>
    <style>
      .calculator{
      margin-left: 50px;
      margin-top: 70px;
      border: solid;;
      border-radius:10px;
      border-color: white;
      width: 430px;
      height: 305px;
    
}
    button{
        background-color:transparent;
        color: azure;
        width: 100px;
        height: 50px;

      
 }
    display{
      background-color: black;
      width:395px;
      height: 50px;
      text-align: right;
    }
   .equals{
      background-color: green;
      width: 204px;
      ;         
    }
    .operator{
      background-color: green;
    }
    .clear{
      background-color: gray;
    }
    .delete{
      background-color: gray;
    }
    .percentage{
       background-color: gray;
    }
    
    
</style>
  </head>
  <body style="background-color: black;">
    <div class="calculator">
      <input type="text" id="display" disabled style="background-color: black;
      width:395px;
      height: 50px;
      text-align: right;
      color:white">
      <div>
        <button class="clear" onclick="document.getElementById('display').value=''">C</button>
        <button class="delete" onclick="document.getElementById('display').value= document.getElementById('display').value.slice(0, -1)">DEL</button>
        <button class="percentage" onclick="document.getElementById('display').value +='/100'" >%</button>
        <button class="operator" onclick="document.getElementById('display').value += '/'">÷</button>
        
 </div>
      <div>
      <button class="button"  onclick="document.getElementById('display').value += '7'">7</button>
      <button class="button" onclick="document.getElementById('display').value += '8'">8</button>
      <button class="button" onclick="document.getElementById('display').value += '9'">9</button>
      <button class="operator" onclick="document.getElementById('display').value += '+'">+</button>
      </div>
      <div>
        <button class="button" onclick="document.getElementById('display').value += '4'">4</button>
        <button class="button" onclick="document.getElementById('display').value += '5'">5</button>
        <button class="button" onclick="document.getElementById('display').value += '6'">6</button>
        <button class="operator" onclick="document.getElementById('display').value += '*'">x</button>
      </div>
      <div>
        <button class="button" onclick="document.getElementById('display').value += '1'">1</button>
        <button class="button" onclick="document.getElementById('display').value += '2'">2</button>
        <button class="button" onclick="document.getElementById('display').value += '3'">3</button>
        <button class="operator" onclick="document.getElementById('display').value +='-'">-</button>
      </div>
      <div>
        <button class="button" onclick="document.getElementById('display').value += '.'">.</button>
        <button class="button" onclick="document.getElementById('display').value += '0'">0</button>
        <button class="equals" onclick="document.getElementById('display').value = eval(document.getElementById('display').value)">=</button>

 </div>

</div>
</body>
</html>

         

