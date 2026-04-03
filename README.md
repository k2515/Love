<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proposal</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
body {
    margin: 0;
    padding: 0;
    font-family: Arial;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    height: 100vh;
    overflow: hidden;
}

.container {
    text-align: center;
    margin-top: 150px;
}

h1 {
    font-size: 40px;
    color: white;
}

.buttons {
    margin-top: 30px;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    margin: 10px;
}

#yesBtn {
    background-color: #28a745;
    color: white;
}

#noBtn {
    background-color: #dc3545;
    color: white;
    position: absolute;
}

/* Popup full screen */
.popup {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #ff4d6d;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 40px;
    visibility: hidden;
}
<div class="container">
    <h1>Do you love me? ❤️</h1>

    <div class="buttons">
        <button id="yesBtn">Yes 💖</button>
        <button id="noBtn">No 😢</button>
    </div>
</div>

<script>

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
    let noBtn = document.getElementById("noBtn");
    let yesBtn = document.getElementById("yesBtn");

    noBtn.addEventListener("mouseover", function () {
        let x = Math.random() * window.innerWidth;
        let y = Math.random() * window.innerHeight;

        noBtn.style.position = "absolute";
        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", function () {
        alert("I love you too 💕");
    });
</script>

</body>
</html>

