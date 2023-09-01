# Any-keyPressed
This is a simple HTML and JavaScript code that allows the user to enter a keyword and then displays the keyword on the screen.
# HOSTED LINK- https://kmsarikasingh.github.io/key-press/
# HTML 
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>KeyPressed</title>

</head>
<body>
    <div class="container">Enter Any KeyWord</div>
    
    <script src="index.js"></script>
</body>
</html>
```
# CSS
```
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Courier New', Courier, monospace;
}
.container{
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-weight: 900;
    font-size: 40px;
}
p,h1{
    margin-top: 10px;
    font-size: 40px;
}
```
# JAVASCRIPT
```
let container = document.querySelector(".container");

document.addEventListener("keydown", function (event) {
    container.innerText = "";
    console.log(event);
    // The parameter event is of the type KeyboardEvent
  	let h1 = document.createElement("h1");
    h1.innerText = ` You Pressed  ${event.key}`;
    let p = document.createElement("p");
    p.innerText = `${event.keyCode}`;
    container.appendChild(h1);
    container.appendChild(p);


});
```
