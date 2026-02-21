<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>My Pharmacy - Inventory Management System</title>
<!-- Font Awesome for Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
.features{
    display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
   
    gap:25px;
}
.features, .features-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}
.features {
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}
.card{
    position: relative;
}


/* HERO HEADER WITH CURVE */
header {
  position: relative;
  background: linear-gradient(135deg,#0d3f66,#1bb98a);
  color: #fff;
  padding: 100px 20px 140px 20px;
  text-align: center;
  overflow: hidden;
}

/* Bottom Curve Shape */
header::after {
  content: "";
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  height: 120px;
  background: #f6f9fb;   /* Same as body background */
  border-top-left-radius: 100% 100px;
  border-top-right-radius: 100% 100px;
}

/* Bigger Title */
header h1 {
  font-size: 48px;
  font-weight: 800;
  margin: 10px 0;
}

header p {
  font-size: 20px;
  opacity: 0.95;
}


.card{
    background:#e8f9f2;   /* light green */
    border-left:5px solid #0b6e4f;
    padding:25px;
    border-radius:12px;
    box-shadow:0 8px 25px rgba(0,0,0,0.08);
    transition:0.3s;
}

.card h3{
    color:#0b6e4f;
}

/* Left green curved border */
.card::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    height: 100%;
    width: 6px;
    background: #0b6e4f;
    border-top-left-radius: 18px;
    border-bottom-left-radius: 18px;
}

.card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.12);
}

.card h3 {
    color: #0b6e4f;
    font-size: 20px;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    gap: 10px;
}

.card p {
    color: #333;
    line-height: 1.6;
}


/* --- RESET & BASE --- */
html, body {
    margin:0;
    padding:0;
    box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: #f6f9fb;
  color:#333;
}

/* HEADER */
header {
  background: linear-gradient(135deg,#0b6e4f,#1bb98a);
  color:#fff;
  padding:60px 20px;
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
  0% { color:#ff4d4d; }
  33% { color:#4da6ff; }
  66% { color:#4dff88; }
  100% { color:#ff4d4d; }
}
.rgb-text {
  display: block;
  font-size: 48px;
  font-weight: 800;
  animation: rgbColor 4s infinite;
  margin-bottom: 10px;
}

/* NAVBAR */
nav {
  background:#064d38;
  padding:12px 20px;
  position: sticky;
  top: 0;
  z-index: 100;
}

.navbar {
  display:flex;
  align-items:center;
  max-width: 1100px;
  margin: 0 auto;
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
  font-size:32px;
  color:#0b6e4f;
  margin-bottom:30px;
  text-align:center;
}

.features, .features-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.card{
    background:#fff;
    border-top:5px solid #0b6e4f;
    padding:25px;
    border-radius:12px;
    box-shadow:0 5px 15px rgba(0,0,0,0.08);
    transition:0.3s;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow:0 12px 25px rgba(0,0,0,0.15);
}

.card h3{
    color:#0b6e4f;
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
  border: none;
  cursor: pointer;
}

.btn:hover {
  transform: scale(1.05);
  box-shadow:0 6px 18px rgba(0,0,0,0.2);
}

/* PRICING */
.pricing-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    margin-top: 20px;
}

.price-card {
    background: white;
    padding: 40px;
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
    text-align: center;
    flex: 1;
    min-width: 280px;
    max-width: 350px;
    border: 1px solid #eee;
    position: relative;
}

.price-card.premium {
    border: 2px solid #1bb98a;
    transform: scale(1.05);
}

.price-card .price {
    font-size: 36px;
    color: #0b6e4f;
    font-weight: bold;
    margin: 15px 0;
}


.price-card ul {
    list-style: none;
    padding: 0;
    text-align: left;
    margin-bottom: 25px;
}

.price-card ul li {
    margin-bottom: 10px;
    color: #555;
}

.price-card ul li i {
    color: #1bb98a;
    margin-right: 8px;
}

/* FLOATING WHATSAPP */
.float-whatsapp {
  position: fixed;
  width: 60px;
  height: 60px;
  bottom: 30px;
  right: 30px;
  background-color: #25D366;
  color: white;
  border-radius: 50px;
  text-align: center;
  font-size: 30px;
  box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: 0.3s;
}

.float-whatsapp:hover {
  background-color: #20b557;
  transform: scale(1.1);
}

/* FOOTER */
footer {
  background:#064d38;
  color:#fff;
  text-align:center;
  padding:30px;
  margin-top: 50px;
}

/* RESPONSIVE */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
        gap: 10px;
    }
    .right-contact {
        margin-left: 0;
        flex-direction: column;
        gap: 10px;
    }
    .rgb-text {
        font-size: 32px;
    }
    .price-card.premium {
        transform: scale(1);
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
  <span class="rgb-text">My Pharmacy</span>
  <h1>Inventory Management System</h1>
  <p>All-in-one billing, GST & inventory software made for medical stores</p>
  <br>
  <a href="#download" class="btn" style="background: white; color: #0b6e4f;">Download Demo</a>
</header>

<!-- NAVBAR -->
<nav>
  <div class="navbar">
    <div class="right-contact">
      <a href="#" onclick="alert('Contact Number: +91-9412561200')">Contact Us</a>
      <a href="tel:+919412561200">📞 +91 9412561200</a>
      <a href="https://wa.me/919412561200?text=Hello%20I%20need%20support"
         class="whatsapp" target="_blank">
        <i class="fab fa-whatsapp"></i> WhatsApp
      </a>
    </div>
  </div>
</nav>

<!-- KEY FEATURES -->
<section class="container">


  <h2 class="section-title">Key Features</h2>
 
   <div class="features">

   <div class="card"> <h3>⚡ Fast Billing</h3> <p>Generate invoices in seconds with shortcut support.</p> </div> <div class="card"> <h3>🧾 GST Ready</h3> <p>Automatic GST, HSN codes, and GSTR reports.</p> </div> <div class="card"> <h3>📦 Stock Control</h3> <p>Batch wise stock, expiry alerts, and low-stock warnings.</p> </div> <div class="card"> <h3>🛒 Purchase Module</h3> <p>Supplier bills, returns, and outstanding tracking.</p> </div> <div class="card"> <h3>👥 Customer Ledger</h3> <p>Credit history, payments, and balance reports.</p> </div> <div class="card"> <h3>📊 Reports</h3> <p>Sales, profit, tax, and monthly analysis reports.</p> </div> </div>

  </div>
</section>

<!-- DOWNLOAD SECTION -->
<div id="download" style="text-align:center; margin: 40px 20px;">
    <a href="https://drive.google.com/uc?export=download&id=1NaMYOnSuCPI3HLGxhBHzctPTVF9Tvle0" class="btn" target="_blank">⬇ Download Free Demo</a>
</div>

<!-- PRICING PLANS -->
<section class="container">
  <h2 class="section-title">Pricing Plans</h2>
  <div class="pricing-container">
    
    <!-- Basic Plan -->
    <div class="price-card">
        <h3>Basic</h3>
        <div class="price">₹2,499</div>
        <p>With 1 Year Support</p>
        <ul>
            <li><i class="fas fa-check"></i> Billing Software</li>
            <li><i class="fas fa-check"></i> GST Reports</li>
            <li><i class="fas fa-check"></i> Stock Management</li>
            <li><i class="fas fa-times" style="color:#ccc"></i> Advanced Analytics</li>
        </ul>
        <a href="https://wa.me/919412561200" target="_blank" class="btn">Contact Now</a>
    </div>

    <!-- Premium Plan -->
    <div class="price-card premium">
        <div style="position:absolute; top:-12px; right:-12px; background:#ff4d4d; color:white; padding:5px 10px; border-radius:20px; font-size:12px; font-weight:bold;">BEST VALUE</div>
        <h3>Premium</h3>
        <div class="price">₹10,000</div>
        <p>One-time payment for 5 Years</p>
        <ul>
           <li><i class="fas fa-check"></i> Billing Software</li>
            <li><i class="fas fa-check"></i> GST Reports</li>
            <li><i class="fas fa-check"></i> Stock Management</li>
            <li><i class="fas fa-times" style="color:#ccc"></i> Advanced Analytics</li>
        </ul>
        <a href="https://wa.me/919412561200" target="_blank" class="btn">Contact Now</a>
    </div>

  </div>
</section>

<!-- WHY CHOOSE US -->
<section class="container">
  <h2 class="section-title">Why Choose Us?</h2>
  <div class="features">
    <div class="card">
        <h3>✔ Easy to Use</h3>
        <p>No training required. Simple interface for fast billing.</p>
    </div>
    <div class="card">
        <h3>✔ Affordable</h3> 
        <p>Flexible one-time pricing with no hidden fees.</p>
    </div>
    <div class="card">
        <h3>✔ Trusted Support</h3>
        <p>Dedicated Phone & WhatsApp support.</p>
    </div>
  </div>
</section>

<!-- BEST WISHES -->
<section class="container">
  <h2 class="section-title">Best Wishes from My Pharmacy</h2>
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




<!-- FLOATING WHATSAPP BUTTON -->
<a href="https://wa.me/919412561200?text=Hello%20I%20need%20Pharmacy%20Software" target="_blank" class="float-whatsapp">
    <i class="fab fa-whatsapp"></i>
</a>

<!-- PARTY MANAGEMENT SECTION -->
<section class="container">
  <h2 class="section-title">Party / Supplier Management</h2>

  <div class="features">

    <div class="card">
      <h3>🏢 Party Master</h3>
      <p>Add & manage party details including Name, Address & Contact Number.</p>
    </div>

    <div class="card">
      <h3>📞 Contact Details</h3>
      <p>Store mobile number, GST number, and city information.</p>
    </div>

    <div class="card">
      <h3>💰 Outstanding Tracking</h3>
      <p>Track pending payments, credit balance & transaction history.</p>
    </div>

  </div>

  <!-- Sample Party Table -->
  <div style="margin-top:40px; overflow-x:auto;">
    <table style="width:100%; border-collapse:collapse; background:white; border-radius:10px; overflow:hidden; box-shadow:0 5px 15px rgba(0,0,0,0.08);">
      <thead style="background:#0b6e4f; color:white;">
        <tbody>
          <tr>
          <th style="padding:12px;">User Party Name</th>
          <th style="padding:12px;">User Address</th>
          <th style="padding:12px;">User Contact Number</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td style="padding:12px;">Sahil Medical Store</td>
          <td style="padding:12px;">Neoar Mata Mandir Kotli Bagich Deori Road Agra</td>
          <td style="padding:12px;">+91 6395283710</td>
        </tr>
        <tr style="background:#f6f9fb;">
          <td style="padding:12px;">Life Care Pharmacy</td>
          <td style="padding:12px;">Madhuvan Plaza Conplex Delhi Gate Agra</td>
          <td style="padding:12px;">+91 7078267474</td>
        </tr>
        <tr>
          <td style="padding:12px;">Medicine Point</td>
          <td style="padding:12px;">Madhuvan Plaza Conplex Delhi Gate Agra</td>
          <td style="padding:12px;">+91 9760216280</td>
        </tr>
        <tr>
 <td style="padding:12px;">Vivek Medical Store</td>
          <td style="padding:12px;">Madhuvan Plaza Conplex Delhi Gate Agra</td>
          <td style="padding:12px;">+91 9079281543</td>
        </tr>

      </tbody>
    </table>
  </div>
</section>


<!-- FOOTER -->
<footer>
    <p>Trusted billing, GST & inventory software for modern Retailers</p>
    <p>&copy; 2026 My Pharmacy Inventory Management System | All Rights Reserved</p>
</footer>
