<!DOCTYPE html>
<html>
<body>


<p id="demo"></p>

<script>
var myObj, myJSON, text, obj;
//Storing data:
myObj = { name: "Visit www.cranfieldandmarstonvale.co.uk for more informtion on these and other news headlines", age: 31, city: "New York" };
myJSON = JSON.stringify(myObj);
localStorage.setItem("testJSON", myJSON);
//Retrieving data:
text = localStorage.getItem("testJSON");
obj = JSON.parse(text);
document.getElementById("demo").innerHTML = obj.name;
</script>

</body>
</html>
