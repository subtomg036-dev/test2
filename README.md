<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Geonation Store</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">

<style>
* {
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
}

body {
  margin: 0;
  background: radial-gradient(circle at top, #2a200f, #0a0907 60%);
  color: #fff;
}

/* HEADER */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 40px;
}

.logo {
  font-size: 22px;
  font-weight: 800;
}

.copy-ip {
  background: #ffffff;
  color: #000;
  border: none;
  padding: 10px 18px;
  border-radius: 14px;
  font-weight: 700;
  cursor: pointer;
  transition: 0.3s;
}

.copy-ip:hover {
  transform: scale(1.05);
}

/* MENU */
.menu {
  display: flex;
  gap: 14px;
  justify-content: center;
  margin-bottom: 10px;
}

.menu button {
  background: #1a1a1a;
  border: none;
  padding: 10px 18px;
  border-radius: 14px;
  color: #fff;
  cursor: pointer;
  transition: 0.3s;
}

.menu button:hover {
  background: #2a2a2a;
  transform: translateY(-2px);
}

/* GRID */
.store {
  padding: 40px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 25px;
}

/* CARD */
.card {
  background: linear-gradient(160deg, #151515, #0c0c0c);
  border-radius: 22px;
  padding: 22px;
  box-shadow: 0 0 40px rgba(0,0,0,0.6);
  transition: 0.35s;
  position: relative;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 0 60px rgba(255,170,0,0.25);
}

.price {
  position: absolute;
  top: 18px;
  right: 18px;
  font-weight: 700;
  opacity: 0.85;
}

.card h2 {
  margin-top: 40px;
  font-size: 20px;
}

.card ul {
  margin: 20px 0;
  padding-left: 0;
  list-style: none;
}

.card ul li {
  opacity: 0.85;
  margin-bottom: 8px;
  font-size: 14px;
}

/* BUY BUTTON */
.buy {
  width: 100%;
  padding: 12px;
  border-radius: 14px;
  border: none;
  font-weight: 700;
  cursor: pointer;
  transition: 0.3s;
}

.buy.orange { background: #ffae00; color: #000; }
.buy.white { background: #fff; color: #000; }

.buy:hover {
  transform: scale(1.05);
}

/* COLORS */
.vip   { border-top: 4px solid #8a2be2; }
.plus  { border-top: 4px solid #ff4040; }
.key   { border-top: 4px solid #00ffaa; }
</style>
</head>

<body>

<header>
  <div class="logo">Geonation</div>
  <button class="copy-ip" onclick="copyIP()">Copy IP</button>
</header>

<div class="menu">
  <button>Store</button>
  <button>VIP Ranks</button>
  <button>Buy Keys</button>
</div>

<section class="store">

  <div class="card vip">
    <div class="price">5 GEL / Monthly</div>
    <h2>VIP</h2>
    <ul>
      <li>✔ Unique Kit</li>
      <li>✔ /fly</li>
      <li>✔ Extra Homes</li>
    </ul>
    <button class="buy white">ყიდვა</button>
  </div>

  <div class="card plus">
    <div class="price">10 GEL / Monthly</div>
    <h2>+VIP</h2>
    <ul>
      <li>✔ All VIP perks</li>
      <li>✔ Better Kit</li>
      <li>✔ Extra Commands</li>
    </ul>
    <button class="buy white">ყიდვა</button>
  </div>

  <div class="card key">
    <div class="price">0.50 GEL</div>
    <h2>Light Key</h2>
    <button class="buy orange">Buy</button>
  </div>

  <div class="card key">
    <div class="price">1 GEL</div>
    <h2>Legendary Key</h2>
    <button class="buy orange">Buy</button>
  </div>

  <div class="card key">
    <div class="price">2 GEL</div>
    <h2>Amethyst Key</h2>
    <button class="buy orange">Buy</button>
  </div>

</section>

<script>
function copyIP() {
  navigator.clipboard.writeText("91.197.6.16:22976");
  alert("IP copied!");
}
</script>

</body>
</html>
