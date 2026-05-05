<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday 🎂</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }body {
  background: linear-gradient(135deg, #ffdde1, #ee9ca7);
  height: 100vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
  color: white;
}

.box {
  width: 140px;
  height: 140px;
  background: #ff4d6d;
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 60px;
  cursor: pointer;
  transition: transform 0.3s;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

.box:hover {
  transform: scale(1.05);
}

.hidden {
  display: none;
}

.cake {
  font-size: 120px;
  cursor: pointer;
  animation: bounce 1s infinite;
}

.message {
  margin-top: 20px;
  font-size: 28px;
  width: 90%;
  max-width: 500px;
  line-height: 1.5;
  animation: fadeIn 2s ease;
}

.choco {
  position: absolute;
  font-size: 35px;
  animation: fall linear infinite;
}

@keyframes bounce {
  0%,100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fall {
  from {
    transform: translateY(-100px);
    opacity: 1;
  }
  to {
    transform: translateY(110vh);
    opacity: 0;
  }
}

.tap-text {
  margin-top: 15px;
  font-size: 18px;
  opacity: 0.9;
}

  </style>
</head>
<body>  <div id="giftSection">
    <div class="box" onclick="openGift()">🎁</div>
    <div class="tap-text">Tap the gift 🎀</div>
  </div>  <div id="cakeSection" class="hidden">
    <div class="cake" onclick="blowCandle()" id="cake">🎂</div>
    <div class="tap-text">Tap the cake to blow candles 🕯️</div>
  </div>  <div id="wishSection" class="hidden">
    <div class="message">
      Happy Birthday Bestie 💖<br><br>
      Tu meri life ki sabse special person hai ✨<br>
      Hamesha aise hi smile karti reh 😊<br><br>
      Stay happy, stay cute 🎂💫
    </div>
  </div>  <script>
    function openGift() {
      document.getElementById('giftSection').classList.add('hidden');
      document.getElementById('cakeSection').classList.remove('hidden');
    }

    function blowCandle() {
      document.getElementById('cake').innerHTML = '🍰';
      document.getElementById('cakeSection').classList.add('hidden');
      document.getElementById('wishSection').classList.remove('hidden');

      for (let i = 0; i < 40; i++) {
        let choco = document.createElement('div');
        choco.classList.add('choco');
        choco.innerHTML = ['🍫','💖','✨','🎉'][Math.floor(Math.random()*4)];
        choco.style.left = Math.random() * 100 + 'vw';
        choco.style.animationDuration = (Math.random() * 3 + 2) + 's';
        document.body.appendChild(choco);
      }
    }
  </script></body>
</html>


<!--
**aryankhalkhanda8630-dev/aryankhalkhanda8630-dev** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
