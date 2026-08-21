<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Pritam 🎂</title>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Poppins", sans-serif;
  overflow: hidden;
  background: linear-gradient(135deg, #12002f, #3b0066, #ff1493);
  color: white;
}

/* ---------- LOGIN ---------- */

#loginPage {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  overflow: hidden;
}

.login-box {
  width: 90%;
  max-width: 420px;
  padding: 40px 30px;
  text-align: center;
  border-radius: 25px;
  background: rgba(255,255,255,0.12);
  backdrop-filter: blur(15px);
  box-shadow: 0 0 50px rgba(255,20,147,.4);
  animation: float 3s ease-in-out infinite;
}

.login-box h1 {
  font-size: 42px;
  margin-bottom: 10px;
}

.login-box p {
  margin-bottom: 25px;
  opacity: .85;
}

input {
  width: 100%;
  padding: 15px;
  border: none;
  border-radius: 30px;
  text-align: center;
  font-size: 17px;
  outline: none;
  margin-bottom: 15px;
}

button {
  border: none;
  padding: 14px 30px;
  border-radius: 30px;
  background: linear-gradient(90deg,#ff1493,#ff69b4);
  color: white;
  font-size: 17px;
  cursor: pointer;
  box-shadow: 0 5px 20px rgba(255,20,147,.5);
  transition: .3s;
}

button:hover {
  transform: scale(1.08);
}

#error {
  color: #ffb3d9;
  margin-top: 15px;
  display: none;
}

/* ---------- MAIN ---------- */

#mainPage {
  display: none;
  height: 100vh;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.section {
  min-height: 100vh;
  display: none;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 25px;
}

.section.active {
  display: flex;
}

/* ---------- BIRTHDAY ---------- */

.birthday-title {
  font-size: clamp(42px, 10vw, 85px);
  color: #fff;
  text-shadow:
    0 0 10px #fff,
    0 0 25px #ff1493,
    0 0 50px #ff1493;
  animation: zoomIn 2s ease;
}

.name {
  font-size: clamp(50px, 13vw, 110px);
  font-weight: 900;
  color: #ffd700;
  text-shadow: 0 0 20px #ff8c00;
  animation: bounce 2s infinite;
}

.subtitle {
  font-size: 20px;
  margin: 20px;
  opacity: .9;
}

/* ---------- CAKE ---------- */

.cake {
  position: relative;
  width: 240px;
  height: 180px;
  margin: 35px auto;
}

.layer {
  position: absolute;
  left: 10px;
  width: 220px;
  height: 55px;
  border-radius: 12px;
  background: linear-gradient(#ff8fc7,#ff4fa3);
  box-shadow: inset 0 -8px rgba(180,0,80,.25);
}

.layer.one { bottom: 0; }
.layer.two { bottom: 48px; width: 190px; left: 25px; }
.layer.three { bottom: 96px; width: 155px; left: 42px; }

.cream {
  position: absolute;
  background: white;
  width: 100%;
  height: 10px;
  border-radius: 50%;
  top: 4px;
}

.candle {
  position: absolute;
  width: 12px;
  height: 50px;
  background: repeating-linear-gradient(
    45deg,
    #fff,
    #fff 6px,
    #ff1493 6px,
    #ff1493 12px
  );
  top: -48px;
  border-radius: 5px;
}

.c1 { left: 75px; }
.c2 { left: 115px; }
.c3 { left: 155px; }

.flame {
  position: absolute;
  width: 20px;
  height: 28px;
  background: #ffd700;
  border-radius: 50% 50% 50% 0;
  transform: rotate(-45deg);
  top: -30px;
  left: -4px;
  box-shadow: 0 0 20px #ff8c00;
  animation: flicker .25s infinite alternate;
}

.cake.cut {
  animation: cakeCut 1.5s forwards;
}

/* ---------- NOTE ---------- */

.note {
  max-width: 750px;
  padding: 40px;
  background: rgba(255,255,255,.12);
  border: 1px solid rgba(255,255,255,.25);
  border-radius: 30px;
  backdrop-filter: blur(15px);
  box-shadow: 0 0 40px rgba(255,20,147,.35);
  animation: noteIn 1.5s ease;
}

.note h2 {
  font-size: 40px;
  color: #ffd700;
  margin-bottom: 20px;
}

.note p {
  font-size: 20px;
  line-height: 1.8;
}

.signature {
  margin-top: 25px;
  font-size: 24px;
  color: #ffb6e1;
}

/* ---------- FLOATING HEARTS ---------- */

.heart {
  position: absolute;
  bottom: -50px;
  font-size: 25px;
  animation: rise linear infinite;
  opacity: .7;
}

/* ---------- ANIMATIONS ---------- */

@keyframes float {
  50% { transform: translateY(-12px); }
}

@keyframes zoomIn {
  from { transform: scale(0); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

@keyframes bounce {
  50% { transform: translateY(-15px); }
}

@keyframes flicker {
  from { transform: rotate(-45deg) scale(.9); }
  to { transform: rotate(-45deg) scale(1.1); }
}

@keyframes cakeCut {
  50% { transform: rotate(4deg) scale(1.08); }
  100% { transform: rotate(0) scale(.95); }
}

@keyframes noteIn {
  from {
    opacity: 0;
    transform: translateY(80px) scale(.8);
  }
  to {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}

@keyframes rise {
  from {
    transform: translateY(0) rotate(0);
    opacity: 0;
  }
  20% { opacity: .8; }
  to {
    transform: translateY(-110vh) rotate(360deg);
    opacity: 0;
  }
}

/* ---------- CONFETTI ---------- */

.confetti {
  position: fixed;
  width: 10px;
  height: 20px;
  top: -30px;
  z-index: 99;
  animation: fall 4s linear forwards;
}

@keyframes fall {
  to {
    transform: translateY(110vh) rotate(720deg);
  }
}

@media(max-width:600px) {
  .login-box {
    padding: 30px 20px;
  }

  .note {
    padding: 25px;
  }

  .note p {
    font-size: 16px;
  }
}
</style>
</head>

<body>

<!-- LOGIN PAGE -->
<div id="loginPage">

  <div class="login-box">
    <div style="font-size:60px;">🎁</div>

    <h1>Special Surprise</h1>

    <p>Someone has prepared a special birthday surprise...</p>

    <input
      type="password"
      id="password"
      placeholder="Enter password"
      onkeypress="if(event.key==='Enter') login()"
    >

    <button onclick="login()">Unlock Surprise 🔐</button>

    <div id="error">Wrong password! Try again ❤️</div>
  </div>

</div>


<!-- MAIN PAGE -->
<div id="mainPage">

  <!-- BIRTHDAY INTRO -->
  <section class="section active" id="intro">

    <div>🎈 🎉 🎈</div>

    <h1 class="birthday-title">
      HAPPY BIRTHDAY
    </h1>

    <div class="name">
      PRITAM ❤️
    </div>

    <p class="subtitle">
      Today is all about YOU! ✨
    </p>

    <button onclick="showCake()">
      Continue to Your Surprise 🎁
    </button>

  </section>


  <!-- CAKE SECTION -->
  <section class="section" id="cakeSection">

    <h1>🎂 It's Cake Time! 🎂</h1>

    <p style="margin-top:10px;">
      Make a wish, Pritam! ✨
    </p>

    <div class="cake" id="cake">

      <div class="candle c1">
        <div class="flame"></div>
      </div>

      <div class="candle c2">
        <div class="flame"></div>
      </div>

      <div class="candle c3">
        <div class="flame"></div>
      </div>

      <div class="layer three">
        <div class="cream"></div>
      </div>

      <div class="layer two">
        <div class="cream"></div>
      </div>

      <div class="layer one">
        <div class="cream"></div>
      </div>

    </div>

    <button onclick="cutCake()">
      🔪 Cut the Cake 🎂
    </button>

  </section>


  <!-- FINAL MESSAGE -->
  <section class="section" id="message">

    <div class="note">

      <h2>💌 A Birthday Note for Pritam</h2>

      <p>
        Dear Pritam,
        <br><br>

        Wishing you a very
        <strong style="color:#ffd700;">
          HAPPY BIRTHDAY! 🎂🎉
        </strong>

        <br><br>

        May this special day bring you endless happiness,
        beautiful memories, success and lots of reasons to smile.

        <br><br>

        May every dream you have come true,
        and may the coming year of your life be even more
        amazing than the last.

        <br><br>

        Keep smiling, keep shining and always stay the
        wonderful person you are. ❤️

        <br><br>

        Here's to another year of adventures,
        laughter and unforgettable moments!

      </p>

      <div class="signature">
        With lots of love ❤️<br>
        Happy Birthday, Pritam! 🎉
      </div>

    </div>

  </section>

</div>


<script>

/* LOGIN */

function login() {

  const password =
    document.getElementById("password").value;

  if(password.toLowerCase() === "pritam") {

    document.getElementById("loginPage").style.display = "none";

    document.getElementById("mainPage").style.display = "block";

    createHearts();

    setTimeout(() => {
      confetti();
    }, 800);

  } else {

    document.getElementById("error").style.display = "block";

  }

}


/* SHOW CAKE */

function showCake() {

  document.getElementById("intro")
    .classList.remove("active");

  document.getElementById("cakeSection")
    .classList.add("active");

}


/* CAKE CUT */

function cutCake() {

  document.getElementById("cake")
    .classList.add("cut");

  /* Blow out candles */

  document.querySelectorAll(".flame")
    .forEach(flame => {
      flame.style.display = "none";
    });

  confetti();

  setTimeout(() => {

    document.getElementById("cakeSection")
      .classList.remove("active");

    document.getElementById("message")
      .classList.add("active");

    confetti();

  }, 1800);

}


/* CONFETTI */

function confetti() {

  const colors = [
    "#ff1493",
    "#ffd700",
    "#00ffff",
    "#7fff00",
    "#ff4500",
    "#ffffff"
  ];

  for(let i = 0; i < 100; i++) {

    const piece =
      document.createElement("div");

    piece.className = "confetti";

    piece.style.left =
      Math.random() * 100 + "vw";

    piece.style.background =
      colors[Math.floor(Math.random() * colors.length)];

    piece.style.animationDuration =
      (Math.random() * 3 + 2) + "s";

    piece.style.transform =
      `rotate(${Math.random()*360}deg)`;

    document.body.appendChild(piece);

    setTimeout(() => {
      piece.remove();
    }, 5000);

  }

}


/* FLOATING HEARTS */

function createHearts() {

  const emojis = ["❤️","💖","💕","💗","✨","🎈"];

  setInterval(() => {

    const heart =
      document.createElement("div");

    heart.className = "heart";

    heart.innerHTML =
      emojis[Math.floor(Math.random() * emojis.length)];

    heart.style.left =
      Math.random() * 100 + "vw";

    heart.style.animationDuration =
      (Math.random() * 5 + 5) + "s";

    document.getElementById("mainPage")
      .appendChild(heart);

    setTimeout(() => {
      heart.remove();
    }, 10000);

  }, 700);

}

</script>

</body>
</html>
