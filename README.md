<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<title>My Phartmacy</title>

<style>
body {
  margin:0;
  font-family:Arial, sans-serif;
  background:#f6f9fb;
  color:#333;
}

/* HEADER */
header {
  background: linear-gradient(135deg,#0b6e4f,#1bb98a);
  color:#fff;
  padding:45px 20px;
  text-align:center;
}

header h1 {
  margin:0;
  font-size:36px;
}

header p {
  font-size:18px;
  margin-top:10px;
}

/* RGB animation */
@keyframes rgbColor {
  0% { color:red; }
  33% { color:#0096ff; }
  66% { color:#00c853; }
  100% { color:red; }
}
.rgb-text {
  animation: rgbColor 3s infinite;
}

/* NAVBAR */
nav {
  background:#064d38;
  padding:12px 20px;
}

.navbar {
  display:flex;
  align-items:center;
}

.right-contact {
  margin-left:auto;
  display:flex;
  align-items:center;
  gap:20px;
}

.right-contact a {
  color:#fff;
  text-decoration:none;
  font-weight:600;
}

.whatsapp {
  color:#25D366;
}

/* CONTENT */
.container {
  max-width:1100px;
  margin:auto;
  padding:40px 20px;
}

.section-title {
  font-size:28px;
  color:#0b6e4f;
  margin-bottom:20px;
  text-align:center;
}

.features {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:20px;
}

.card {
  background:#fff;
  padding:20px;
  border-radius:10px;
  box-shadow:0 4px 12px rgba(0,0,0,0.08);
  transition:0.3s;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow:0 8px 20px rgba(0,0,0,0.15);
}

.card h3 {
  color:#1bb98a;
  margin-top:0;
}

/* BUTTON */
.btn {
  display:inline-block;
  background: linear-gradient(135deg,#0b6e4f,#1bb98a);
  color:white;
  padding:12px 24px;
  border-radius:5px;
  text-decoration:none;
  font-weight:bold;
  transition:0.3s;
}

.btn:hover {
  transform: scale(1.05);
  box-shadow:0 6px 18px rgba(0,0,0,0.2);
}

/* FOOTER */
footer {
  background:#064d38;
  color:#fff;
  text-align:center;
  padding:25px;
}
</style>
</head>

<body>

<header>
  <h1 class="rgb-text">My Phartmacy </h1>
<br>
<h1 class="text"> Inventory Management System</h1>
  <p>All-in-one billing, GST & inventory software made for medical stores</p>
</header>

<nav>
  <div class="navbar">
    <div class="right-contact">
      <a href="#" onclick="alert('Contact Number: +91-9412561200')">Contact Us</a>
      <a href="tel:+919412561200">📞 +91 9412561200</a>
      <a href="https://wa.me/919412561200?text=Hello%20I%20need%20support"
         class="whatsapp" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg"
             width="20" style="vertical-align:middle;">
        WhatsApp
      </a>
    </div>
  </div>
</nav>

<section class="container">
  <h2 class="section-title">Key Features</h2>

  <div class="features">
    <div class="features">
    <div class="card"><h3>⚡ Fast Billing</h3><p>Generate invoices in seconds with shortcut support.</p></div>
    <div class="card"><h3>🧾 GST Ready</h3><p>Automatic GST, HSN codes, and GSTR reports.</p></div>
    <div class="card"><h3>📦 Stock Control</h3><p>Batch‑wise stock, expiry alerts, and low‑stock warnings.</p></div>
    <div class="card"><h3>🛒 Purchase Module</h3><p>Supplier bills, returns, and outstanding tracking.</p></div>
    <div class="card"><h3>👥 Customer Ledger</h3><p>Credit history, payments, and balance reports.</p></div>
    <div class="card"><h3>📊 Reports</h3><p>Sales, profit, tax, and monthly analysis reports.</p></div>
  </div>


 

<div id="download" style="text-align:center;margin-top:35px">
    <a href="https://drive.google.com/uc?export=download&id=1NaMYOnSuCPI3HLGxhBHzctPTVF9Tvle0" class="btn" target="_blank">⬇ Download Free Demo</a>
  </div>
</section>

<section class="container">
  <h2 class="section-title">Why Choose {Retailers}?</h2>
  <div class="features">
    <div class="card"><h3>✔ Easy to Use</h3><p>No training required</p></div>
   <div class="card">  <h3>✔ Affordable</h3> <p>Flexible yearly or one-time pricing with no hidden fees</p></div>
    <div class="card"><h3>✔ Trusted Support</h3><p>Phone & WhatsApp support</p></div>
  </div>
</section>

<section class="container">
  <h2 class="section-title">Best Wishes from {Retailers}</h2>
  <div class="features">
    <div class="card">
      <h3>🚀 Grow With Confidence</h3>
      <p>We wish your pharmacy steady growth, smooth billing, and zero stress operations.</p>
    </div>
    <div class="card">
      <h3>🤝 Long-Term Partnership</h3>
      <p>Our goal is not just software, but a trusted relationship with every retailer.</p>
    </div>
    <div class="card">
      <h3>💊 Built for Indian Pharmacies</h3>
      <p>Designed keeping real medical store needs in mind.</p>
    </div>
  </div>
</section>



<footer>
<p>Trusted billing, GST & inventory software for modern Retailers</p>

© 2026 My Phartmacy Inventory Management System | Built for Retailers

</footer>

</body>
</html>
