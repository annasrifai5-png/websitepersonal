<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8" />
<title>Upgrade Relationship</title>
<style>
    body {
        background: radial-gradient(circle at top, #001f3f, #000814);
        color: #00d9ff;
        font-family: 'Courier New', monospace;
        text-align: center;
        padding-top: 100px;
    }
    .box {
        border: 2px solid #00d9ff;
        padding: 20px;
        display: inline-block;
        background: rgba(0, 0, 50, 0.5);
        box-shadow: 0 0 20px #00d9ff;
    }
    button {
        padding: 10px 20px;
        margin: 10px;
        font-size: 18px;
        cursor: pointer;
        border: none;
        box-shadow: 0 0 10px #00d9ff;
        background: #003b5c;
        color: #00d9ff;
    }
    #message {
        margin-top: 30px;
        font-size: 24px;
        color: #00ffea;
    }
</style>
</head>
<body>

<div class="box">
    <h2>ERROR: Teman biasa NOT FOUND</h2>
    <p>Upgrade ke PACAR?</p>
    <button onclick="yesClick()">YES</button>
    <button onclick="noClick()">NO</button>
</div>

<p id="message"></p>

<audio id="levelUpSound">
    <source src="https://actions.google.com/sounds/v1/cartoon/wood_plank_flicks.ogg" type="audio/ogg">
</audio>

<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
<script>
function yesClick() {
    document.getElementById("levelUpSound").play();
    confetti();
    document.getElementById("message").innerText = "🎉 RESMI JADIAN! 🎉";
}

function noClick() {
    document.getElementById("message").innerText = "Kok NO? Coba lagi 😤";
}
</script>

</body>
</html>
