# Hugg-😭
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Hug Day Saeee</title>

<style>
    body {
        margin: 0;
        padding: 0;
        font-family: 'Segoe UI', sans-serif;
        background: linear-gradient(135deg, #ff9a9e, #fad0c4);
        text-align: center;
        color: #fff;
        overflow: hidden;
    }

    h1 {
        margin-top: 40px;
        font-size: 2.5rem;
    }

    h2 {
        font-weight: normal;
        margin-top: 10px;
    }

    .card {
        background: rgba(255,255,255,0.2);
        margin: 40px auto;
        padding: 25px;
        width: 90%;
        max-width: 420px;
        border-radius: 25px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.3);
    }

    .card p {
        font-size: 1.1rem;
        line-height: 1.7;
    }

    button {
        margin-top: 15px;
        padding: 12px 28px;
        font-size: 1rem;
        border: none;
        border-radius: 30px;
        background: #ffffff;
        color: #ff4d6d;
        cursor: pointer;
        transition: 0.3s;
        font-weight: bold;
    }

    button:hover {
        transform: scale(1.08);
        background: #ffe0ec;
    }

    .heart {
        position: fixed;
        top: -40px;
        font-size: 26px;
        animation: fall linear infinite;
    }

    @keyframes fall {
        0% { transform: translateY(0); opacity: 1; }
        100% { transform: translateY(110vh); opacity: 0; }
    }
</style>
</head>

<body>

<h1>🤗 Happy Hug Day 🤗</h1>
<h2>For My Saeee 💕</h2>

<div class="card">
    <p>
        Saeee ❤️<br><br>
        A hug from you feels like home,<br>
        where all worries disappear 🤍<br><br>

        On this Hug Day,<br>
        I just want to hold you tight<br>
        and never let go 💞<br><br>

        Whenever you feel low,<br>
        remember my arms are always open for you 🤗
    </p>

    <button onclick="sendHug()">Send You a Hug 🤗</button><br>
    <button onclick="realHug()">Come Here 🫶</button>
</div>

<script>
function sendHug() {
    alert("Saeee 🤗 Sending you the warmest hug filled with love and comfort 💖");
}

function realHug() {
    alert("Come here Saeee 🥺🤍 Let me hug you tight and make everything better 💕");
}

// Floating hearts animation
setInterval(() => {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDuration = (3 + Math.random() * 3) + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 6000);
}, 300);
</script>

</body>
</html>
