<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title></title>
</head>
<body>
	<script type="text/javascript">
		const calculator = {
			add: (a, b) => a + b,
			subtract: (a, b) => a - b,
			multiply: (a, b) => a * b,
			divide: (a, b) => {
				if (b === 0) {
					throw new Error("Cannot divide by zero");
				}
				return a / b;
			}
		};

		try{
		const resultAdd = calculator.add(35, 34);
		const resultSubtract = calculator.subtract(100, 31);
		const resultMultiply = calculator.multiply(3, 23); 

			const resultDivide = calculator.divide(138, 2);

			console.log(resultAdd, resultSubtract, resultMultiply, resultDivide);
		}catch (error){
			console.error(error.message);
		}
	</script>
	

</body>
</html>
