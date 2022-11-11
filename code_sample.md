<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fizz Buzz</title>
<script>

function fizzbuzz() {
	var display = document.getElementById('display');
	var displayHTML = "";
	for (i = 0; i < 100; i++) {

		if(i % 3==0 && i % 5==0){	//if the val divisible by 3 and 5
					displayHTML+= "<p>"+"FizzBuzz"+"</p>";
		}
		else if(i % 5==0){				//if the val divisible by 5
					displayHTML += "<p>"+"Buzz"+"</p>";
		}
		else if(i % 3==0){
					displayHTML += "<p>"+"Fizz"+"</p>";		//if the val divisible by 3
		}
		else{
			continue;		//continue if not
		}
	}
	display.innerHTML = displayHTML
}

</script>

</head>

<body onload="fizzbuzz()">
<div id="display">

</div>
</body>

</html>
