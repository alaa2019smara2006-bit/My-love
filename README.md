<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>MY LOVE LOOLETOOO ❤️💍🥹</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: radial-gradient(circle at top, #ffd1dc, #ff9a9e, #fad0c4);
      font-family: 'Poppins', sans-serif;
      overflow: hidden;
    }
    .card {
      background: rgba(255,255,255,0.95);
      padding: 48px 56px;
      border-radius: 28px;
      box-shadow: 0 30px 60px rgba(0,0,0,0.25);
      text-align: center;
      max-width: 420px;
      animation: float 3.2s ease-in-out infinite;
      position: relative;
    }
    h1 {
      margin: 0;
      font-family: 'Playfair Display', serif;
      font-size: 2.4rem;
      color: #e63946;
      letter-spacing: 1px;
    }
    .emojis {
      font-size: 2.2rem;
      margin-top: 14px;
    }
    .subtitle {
      margin-top: 14px;
      color: #555;
      font-weight: 300;
    }
    .date {
      margin-top: 18px;
      font-size: 0.9rem;
      color: #888;
    }
    .heart {
      position: absolute;
      color: rgba(230,57,70,0.25);
      animation: rise 6s linear infinite;
      font-size: 18px;
    }
    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }
    @keyframes rise {
      0% { transform: translateY(0) scale(1); opacity: 0; }
      10% { opacity: 1; }
      100% { transform: translateY(-120vh) scale(1.6); opacity: 0; }
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>MY LOVE LOOLETOOO</h1>
    <div class="emojis">❤️💍🥹</div>
    <div class="subtitle">Forever & Always</div>
    <div class="date">Made with love</div>
  </div>

  <script>
    // floating hearts
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.textContent = '❤';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.bottom = '-20px';
      heart.style.animationDuration = (4 + Math.random() * 4) + 's';
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 8000);
    }
    setInterval(createHeart, 500);
  </script>
</body>
</html>
