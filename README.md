<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kibble Gaming</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Arial', sans-serif;
    }

    body {
      background: #0b0b0f;
      color: white;
      overflow-x: hidden;
    }

    /* HERO SECTION */
    .hero {
      height: 100vh;
      width: 100%;
      background: url('hero.jpg') center/cover no-repeat;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    /* dark overlay like storm/fire mood */
    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle at center, rgba(0,0,0,0.3), rgba(0,0,0,0.95));
    }

    .hero-content {
      position: relative;
      z-index: 2;
    }

    .title {
      font-size: 4rem;
      letter-spacing: 6px;
      text-transform: uppercase;
      color: #ff3b1f;
      text-shadow: 0 0 20px #ff3b1f, 0 0 40px #000;
    }

    .subtitle {
      margin-top: 15px;
      font-size: 1.3rem;
      color: #ccc;
    }

    .btn {
      margin-top: 25px;
      display: inline-block;
      padding: 12px 25px;
      border: 2px solid #ff3b1f;
      color: white;
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 2px;
      transition: 0.3s;
      box-shadow: 0 0 15px rgba(255, 59, 31, 0.4);
    }

    .btn:hover {
      background: #ff3b1f;
      box-shadow: 0 0 30px #ff3b1f;
    }

    /* SECTION */
    .section {
      padding: 80px 20px;
      text-align: center;
      background: linear-gradient(to bottom, #0b0b0f, #111);
    }

    .section h2 {
      color: #ff3b1f;
      margin-bottom: 20px;
      letter-spacing: 3px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }

    .card {
      background: rgba(255,255,255,0.05);
      padding: 20px;
      border: 1px solid rgba(255,59,31,0.3);
      box-shadow: 0 0 20px rgba(255,59,31,0.1);
    }

    footer {
      text-align: center;
      padding: 30px;
      background: #000;
      color: #666;
    }
  </style>
</head>
<body>

  <div class="hero">
    <div class="hero-content">
      <div class="title">KIBBLE GAMING</div>
      <div class="subtitle">Chaos • Survival • Darkness • Community</div>
      <a href="#about" class="btn">Enter the Pack</a>
    </div>
  </div>

  <div id="about" class="section">
    <h2>ABOUT</h2>
    <p>
      Welcome to Kibble Gaming — a dark, high-energy gaming brand built around survival games,
      chaos streams, and a loyal community pack.
    </p>

    <div class="cards">
      <div class="card">🦖 ARK Survival Servers</div>
      <div class="card">⛏️ Minecraft Modding</div>
      <div class="card">🚗 Simulator Chaos</div>
      <div class="card">💀 Dark Themed Branding</div>
    </div>
  </div>

  <div class="section">
    <h2>JOIN THE PACK</h2>
    <p>Connect with the community and join the chaos.</p>
    <a href="https://discord.gg/" class="btn">Discord</a>
  </div>

  <footer>
    © 2026 Kibble Gaming • Built in the darkness
  </footer>

</body>
</html>
