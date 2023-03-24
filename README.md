# Calculadora
Fiz uma calculadora utilizando javascript
<!DOCTYPE html>
<html>
<head>
	<title>Micro Calculadora</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<style type="text/css">
		input[type=number]{
			width: 100%;
			padding: 12px 20px;
			margin: 8px 0;
			box-sizing: border-box;
			border: 2px solid #ccc;
			border-radius: 4px;
			background-color: #f8f8f8;
			font-size: 20px;
		}

		input[type=button]{
			background-color: #4CAF50;
			border: none;
			color: white;
			padding: 16px 32px;
			text-decoration: none;
			margin: 4px 2px;
			cursor: pointer;
			font-size: 20px;
		}
	</style>
</head>
<body>
	<h2>Micro Calculadora</h2>
	<input type="number" id="num1" placeholder="Digite o primeiro número">
	<input type="number" id="num2" placeholder="Digite o segundo número">

	<input type="button" value="+" onclick="add()">
	<input type="button" value="-" onclick="sub()">
	<input type="button" value="*" onclick="mul()">
	<input type="button" value="/" onclick="div()">

	<p id="result"></p>

	<script type="text/javascript">
		function add(){
			var num1 = parseInt(document.getElementById('num1').value);
			var num2 = parseInt(document.getElementById('num2').value);
			var result = num1 + num2;
			document.getElementById('result').innerHTML = "Resultado: " + result;
		}

		function sub(){
			var num1 = parseInt(document.getElementById('num1').value);
			var num2 = parseInt(document.getElementById('num2').value);
			var result = num1 - num2;
			document.getElementById('result').innerHTML = "Resultado: " + result;
		}

		function mul(){
			var num1 = parseInt(document.getElementById('num1').value);
			var num2 = parseInt(document.getElementById('num2').value);
			var result = num1 * num2;
			document.getElementById('result').innerHTML = "Resultado: " + result;
		}

		function div(){
			var num1 = parseInt(document.getElementById('num1').value);
			var num2 = parseInt(document.getElementById('num2').value);
			var result = num1 / num2;
			document.getElementById('result').innerHTML = "Resultado: " + result;
		}
	</script>
</body>
</html>
