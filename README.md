<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Kibble Gaming</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;900&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Cinzel', serif;
}

body {
  background: #0a0a0f;
  color: white;
  overflow-x: hidden;
}

/* Lightning background */
body::before {
  content: "";
  position: fixed;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle at 50% 30%, rgba(255,140,0,0.2), transparent 40%),
              radial-gradient(circle at 20% 70%, rgba(0,180,255,0.15), transparent 40%);
  animation: pulse 6s infinite alternate;
  z-index: -2;
}

@keyframes pulse {
  from { transform: scale(1); filter: brightness(1); }
  to { transform: scale(1.1); filter: brightness(1.3); }
}

/* Hero */
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 20px;
}

.hero img {
  width: 300px;
  max-width: 80%;
  filter: drop-shadow(0 0 25px orange);
}

.hero h1 {
  font-size: 60px;
  letter-spacing: 3px;
  margin-top: 20px;
  text-shadow: 0 0 20px orange;
}

.hero p {
  margin-top: 10px;
  opacity: 0.8;
}

/* Button */
.btn {
  margin-top: 25px;
  padding: 15px 30px;
  border: 2px solid orange;
  color: white;
  text-decoration: none;
  font-weight: bold;
  transition: 0.3s;
}

.btn:hover {
  background: orange;
  color: black;
  box-shadow: 0 0 25px orange;
}

/* Sections */
section {
  padding: 80px 20px;
  text-align: center;
}

h2 {
  color: orange;
  margin-bottom: 20px;
  text-shadow: 0 0 10px orange;
}

/* Cards */
.card {
  background: rgba(255,255,255,0.05);
  padding: 20px;
  margin: 10px auto;
  max-width: 600px;
  border-left: 3px solid orange;
}
</style>
</head>

<body>

<div class="hero">
  <!-- replace with your logo file -->
  <img src="logo.png" alt="Kibble Gaming Logo">

  <h1>KIBBLE GAMING</h1>
  <p>Enter the battlefield. Watch the rise of legends.</p>

  <a class="btn" href="https://www.twitch.tv/KibbleGaming" target="_blank">
    WATCH LIVE ON TWITCH
  </a>
</div>

<section>
  <h2>ABOUT</h2>
  <div class="card">
    A dark gaming realm built around survival, chaos, and legendary gameplay.
    Join the pack and witness streams built for warriors.
  </div>
</section>

<section>
  <h2>SCHEDULE</h2>
  <div class="card">
    Streams: TBD (you can add days/times later)
  </div>
</section>

<section>
  <h2>SOCIALS</h2>
  <div class="card">
    Twitch • YouTube • Discord (add your links here)
  </div>
</section>

</body>
</html>
