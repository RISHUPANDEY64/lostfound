<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Proposal 💖</title>

<style>
    body {
        margin: 0;
        padding: 0;
        height: 100vh;
        background: #ffd6e8; /* light pink */
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: Arial, sans-serif;
        overflow: hidden;
    }

    .card {
        background: white;
        padding: 40px;
        border-radius: 15px;
        text-align: center;
        width: 320px;
        position: relative;
    }

    h1 {
        color: hotpink;
        font-size: 42px;
        margin-bottom: 10px;
    }

    p {
        font-size: 18px;
        margin-bottom: 25px;
    }

    button {
        padding: 10px 22px;
        font-size: 16px;
        border: none;
        border-radius: 8px;
        cursor: pointer;
    }

    #yesBtn {
        background: hotpink;
        color: white;
    }

    #noBtn {
        background: #ddd;
        position: absolute;
    }

    #message {
        margin-top: 20px;
        font-weight: bold;
        color: hotpink;
    }
</style>
</head>

<body>

<div class="card">
    <h1>Shivani</h1>
    <p>Shivani will you my valentine? 💖</p>

    <button id="yesBtn">YES</button>
    <button id="noBtn" style="left:180px; top:220px;">NO</button>

    <div id="message"></div>
</div>

<script>
    let noCount = 0;
    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");
    const message = document.getElementById("message");

    noBtn.addEventListener("mouseenter", moveNo);
    noBtn.addEventListener("click", moveNo);

    function moveNo() {
        noCount++;

        if (noCount === 1) {
            message.innerText = "Please… one try 🥺";
        }

        if (noCount >= 6) {
            noBtn.innerText = "YES";
            noBtn.style.background = "hotpink";
            noBtn.style.color = "white";

            noBtn.removeEventListener("mouseenter", moveNo);
            noBtn.removeEventListener("click", moveNo);

            noBtn.onclick = () => {
                message.innerText = "Thank you ❤️";
            };
            return;
        }

        const x = Math.random() * (window.innerWidth - 100);
        const y = Math.random() * (window.innerHeight - 50);

        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    }

    yesBtn.onclick = () => {
        message.innerText = "Thank you ❤️";
    };
</script>

</body>
</html>