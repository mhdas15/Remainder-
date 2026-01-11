# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Zaitoon Reminder 🎉</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: #2b1a12;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-family: Arial, sans-serif;
      text-align: center;
    }
    h1 { font-size: 2.5rem; }
    p { font-size: 1.2rem; }
  </style>
</head>
<body>

<div>
  <h1>🍽️ Zaitoon Reminder</h1>
  <p>Just a few hours to go!</p>
  <p>Get ready to enjoy good food and good company 😄</p>
</div>

<!-- Confetti -->
<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

<!-- Sound -->
<audio id="popSound" autoplay>
  <source src="https://www.soundjay.com/party/party-horn-01.mp3" type="audio/mpeg">
</audio>

<script>
  window.onload = () => {
    confetti({ particleCount: 150, spread: 80, origin: { y: 0.6 } });
    setTimeout(() => {
      confetti({ particleCount: 100, spread: 120, origin: { x: 0.2, y: 0.4 } });
      confetti({ particleCount: 100, spread: 120, origin: { x: 0.8, y: 0.4 } });
    }, 600);
  };
</script>

</body>
</html>