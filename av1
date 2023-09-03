<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>Calculadora de Gorjeta</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-image: linear-gradient(45deg,blue,red);
            margin: 0;
            padding: 0;
        }

        .container {
            background-image: linear-gradient(45deg,white, white);
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }

        .input-group {
            margin: 10px 0;
        }

        label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }

        input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 3px;
        }

        button {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 15px 30px;
            border-radius: 3px;
            cursor: pointer;
        }

        .results {
            margin-top: 20px;
        }

        .results p {
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Calculadora de Gorjeta</h1>
        <div class="input-group">
            <label for="bill">Total da conta: $</label>
            <input type="number" id="bill" placeholder="Digite o total da conta">
        </div>
        <div class="input-group">
            <label for="percentage">Porcentagem da gorjeta:</label>
            <input type="number" id="percentage" placeholder="Digite a porcentagem da gorjeta">
        </div>
        <button id="calculate">Calcular Gorjeta</button>
        <div class="results">
            <p>Gorjeta: $<span id="tipAmount">0.00</span></p>
            <p>Total a pagar: $<span id="totalAmount">0.00</span></p>
        </div>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const calculateButton = document.getElementById("calculate");
            calculateButton.addEventListener("click", calculateTip);
        });

        function calculateTip() {
            const billAmount = parseFloat(document.getElementById("bill").value);
            const tipPercentage = parseFloat(document.getElementById("percentage").value);

            if (isNaN(billAmount) || isNaN(tipPercentage)) {
                alert("Por favor, insira valores válidos.");
                return;
            }

            const tipAmount = (billAmount * (tipPercentage / 100)).toFixed(2);
            const totalAmount = (billAmount + parseFloat(tipAmount)).toFixed(2);

            document.getElementById("tipAmount").textContent = tipAmount;
            document.getElementById("totalAmount").textContent = totalAmount;
        }
    </script>
</body>
</html>
