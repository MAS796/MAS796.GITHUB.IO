# MAS<!DOCTYPE html>
<html>
<head>
    <title>Arithmetic Operations</title>
    <link rel="stylesheet" href="styles.css" />
</head>
<body>
    <h1>Arithmetic Operations</h1>
    <form id="calcForm">
        <input type="number" id="num1" placeholder="Enter first number" required>
        <input type="number" id="num2" placeholder="Enter second number" required>
        <select id="operation">
            <option value="add">Add</option>
            <option value="subtract">Subtract</option>
            <option value="multiply">Multiply</option>
            <option value="divide">Divide</option>
        </select>
        <button type="button" onclick="calculate()">Calculate</button>
    </form>
    <p id="result"></p>

    <script>
        function calculate() {
            const num1 = parseFloat(document.getElementById('num1').value);
            const num2 = parseFloat(document.getElementById('num2').value);
            const operation = document.getElementById('operation').value;
            let result;

            switch (operation) {
                case 'add':
                    result = num1 + num2;
                    break;
                case 'subtract':
                    result = num1 - num2;
                    break;
                case 'multiply':
                    result = num1 * num2;
                    break;
                case 'divide':
                    result = num2 !== 0 ? num1 / num2 : 'Cannot divide by zero';
                    break;
                default:
                    result = 'Invalid operation';
            }

            document.getElementById('result').innerText = 'Result: ' + result;
        }
    </script>
</body>
</html>796.GITHUB.IO
Lab programs 
