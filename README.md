# GTKind.github.io
`AI for people of goodwill`
`Goodwill encompasses attitudes and actions that reflect love, kindness, righteousness, integrity, and the pursuit of peace. It emphasizes the importance of treating others with respect, compassion, and fairness, aligning with the teachings and values found in the Scriptures.`
# Calculator
<html>
<head>
  <title>Calculator</title>
  <style>
    .calculator {
      width: 200px;
      margin: 20px auto;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      text-align: center;
    }

    .calculator input[type="text"] {
      width: 100%;
      margin-bottom: 10px;
      padding: 5px;
    }

    .calculator input[type="button"] {
      width: 48%;
      margin: 5px;
      padding: 10px;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <div class="calculator">
    <input type="text" id="result" readonly>
    <input type="button" value="1" onclick="appendToResult('1')">
    <input type="button" value="2" onclick="appendToResult('2')">
    <input type="button" value="3" onclick="appendToResult('3')">
    <input type="button" value="+" onclick="appendToResult('+')">
    <br>
    <input type="button" value="4" onclick="appendToResult('4')">
    <input type="button" value="5" onclick="appendToResult('5')">
    <input type="button" value="6" onclick="appendToResult('6')">
    <input type="button" value="-" onclick="appendToResult('-')">
    <br>
    <input type="button" value="7" onclick="appendToResult('7')">
    <input type="button" value="8" onclick="appendToResult('8')">
    <input type="button" value="9" onclick="appendToResult('9')">
    <input type="button" value="*" onclick="appendToResult('*')">
    <br>
    <input type="button" value="0" onclick="appendToResult('0')">
    <input type="button" value="." onclick="appendToResult('.')">
    <input type="button" value="=" onclick="calculateResult()">
    <input type="button" value="/" onclick="appendToResult('/')">
    <br>
    <input type="button" value="Clear" onclick="clearResult()">
  </div>

  <script>
    function appendToResult(value) {
      document.getElementById('result').value += value;
    }

    function calculateResult() {
      var result = document.getElementById('result').value;
      var calculatedResult = eval(result);
      document.getElementById('result').value = calculatedResult;
    }

    function clearResult() {
      document.getElementById('result').value = '';
    }
  </script>
</body>
</html>
