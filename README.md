<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>WASH KATBGHINI? 💕</title>

<style>
body {
    margin: 0;
    font-family: Arial;
    background: linear-gradient(135deg, #ffeef8, #ffd6e7, #ffcccb);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
}

/* Hearts */
.heart {
    position: absolute;
    color: #ff1493;
    animation: float 6s linear infinite;
}
@keyframes float {
    from {transform: translateY(100vh);}
    to {transform: translateY(-10vh);}
}

/* Box */
.box {
    text-align: center;
}

h1 {
    color: #ff1493;
}

/* Buttons */
button {
    padding: 15px 25px;
    margin: 10px;
    border: none;
    border-radius: 30px;
    font-size: 18px;
    cursor: pointer;
}

#yes {
    background: #ff1493;
    color: white;
}

#no {
    background: pink;
}

/* Hidden text */
#love {
    display: none;
    font-size: 30px;
    color: #ff1493;
}
</style>
</head>

<body>

<div class="box">
    <h1>WASH KATBGHINI? 💕</h1>

    <button id="yes">AH 💖</button>
    <button id="no">LA 😏</button>

    <div id="love">ANA TANBGHIK BZZEF 😍</div>
</div>

<script>
const yes = document.getElementById("yes");
const no = document.getElementById("no");
const love = document.getElementById("love");

yes.onclick = () => {
    love.style.display = "block";
};

// Move NO button 😆
no.onmouseover = () => {
    no.style.position = "absolute";
    no.style.left = Math.random() * window.innerWidth + "px";
    no.style.top = Math.random() * window.innerHeight + "px";
};

// Hearts animation
setInterval(() => {
    const heart = document.createElement("div");
    heart.innerHTML = "💕";
    heart.className = "heart";
    heart.style.left = Math.random() * 100 + "vw";
    document.body.appendChild(heart);

    setTimeout(() => heart.remove(), 5000);
}, 300);
</script>

</body>
</html>
