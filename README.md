<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love Proposal ❤️</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">
    <h1>Do you love me? 💖</h1>

    <div class="buttons">
        <button id="yesBtn">Yes 😍</button>
        <button id="noBtn">No 😢</button>
    </div>
</div>

<div class="popup" id="popup">
    <h1>I Love You So Much ❤️🥰</h1>
</div>

<script src="script.js"> 
let noBtn = document.getElementById("noBtn");
let yesBtn = document.getElementById("yesBtn");
let popup = document.getElementById("popup");

// Move NO button randomly
noBtn.addEventListener("mouseover", function () {
    let x = Math.random() * (window.innerWidth - 100);
    let y = Math.random() * (window.innerHeight - 100);

    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});

// Show love message
yesBtn.addEventListener("click", function () {
    popup.style.visibility = "visible";
});
</script>

</body>
</html>
