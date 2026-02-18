<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pharmacy Management System</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Poppins',sans-serif;
    background:#f4f7fa;
    color:#333;
}
.float-whatsapp {
   display: none;
}
.float-whatsapp {
   pointer-events: none;
   opacity: 0.6;
}


.float-whatsapp {
   position: fixed;
   bottom: 20px;
   right: 20px;
}
.float-whatsapp {
   position: static;
}

/* HEADER */
header{
    background:linear-gradient(135deg,#0b6e4f,#1bb98a);
    color:white;
    padding:70px 20px;
    text-align:center;
}

header h1{
    font-size:42px;
}

header p{
    margin-top:15px;
    font-size:18px;
    opacity:0.9;
}

/* NAV */
nav{
    background:#064d38;
    padding:15px 20px;
}

.navbar{
    max-width:1100px;
    margin:auto;
    display:flex;
    align-items:center;
}

.logo{
    color:white;
    font-weight:700;
    font-size:20px;
}

.menu{
    margin-left:auto;
    display:flex;
    gap:25px;
}

.menu a{
    color:white;
    text-decoration:none;
    font-weight:500;
    transition:0.3s;
}

.menu a:hover{
    color:#1bb98a;
}

/* SECTION */
.section{
    max-width:1100px;
    margin:auto;
    padding:60px 20px;
}

.section h2{
    text-align:center;
    margin-bottom:40px;
    color:#0b6e4f;
}

/* FEATURES */
.features{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.card{
    background:white;
    padding:25px;
    border-radius:12px;
    box-shadow:0 8px 25px rgba(0,0,0,0.08);
    transition:0.3s;
}

.card:hover{
    transform:translateY(-8px);
}

.card i{
    font-size:30px;
    color:#1bb98a;
    margin-bottom:15px;
}

/* PRICING */
.pricing{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.price-card{
    background:white;
    padding:30px;
    border-radius:15px;
    text-align:center;
    box-shadow:0 8px 25px rgba(0,0,0,0.08);
}

.price{
    font-size:28px;
    font-weight:bold;
    margin:15px 0;
    color:#0b6e4f;
}

.btn{
    display:inline-block;
    background:linear-gradient(135deg,#0b6e4f,#1bb98a);
    color:white;
    padding:12px 25px;
    border-radius:30px;
    text-decoration:none;
    font-weight:600;
    transition:0.3s;
}

.btn:hover{
    transform:scale(1.05);
}
.float-whatsapp {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 60px;
    height: 60px;
    background: #25D366;
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 28px;
    text-decoration: none;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    z-index: 1000;
    transition: 0.3s;
}

.float-whatsapp:hover {
    transform: scale(1.1);
}


/* CONTACT */
.contact{
    text-align:center;
}

.contact a{
    display:inline-block;
    margin:10px;
    color:#0b6e4f;
    font-weight:600;
    text-decoration:none;
}

/* FOOTER */
footer{
    background:#064d38;
    color:white;
    text-align:center;
    padding:25px;
    margin-top:40px;
}

@media(max-width:768px){
    header h1{
        font-size:28px;
    }
}

</style>
</head>

<body>

<nav>
<div class="navbar">
<div class="logo">💊 My-Pharmacy Software</div>
<div class="menu">
<a href="#about">About</a>
<a href="#features">Features</a>
<a href="#pricing">Pricing</a>
<a href="#contact">Contact</a>
</div>
</div>
</nav>

<header>
<h1>Pharmacy Management System</h1>
<p>Complete Billing, GST & Inventory Solution for Medical Stores</p>
<br>
<!--<a href="#" class="btn">Download Free Demo</a> -->
<div id="download" style="text-align:center;margin-top:35px">
    <a href="https://drive.google.com/uc?export=download&id=1NaMYOnSuCPI3HLGxhBHzctPTVF9Tvle0" class="btn" target="_blank">⬇ Download Free Demo</a>
  </div>
</header>

<section id="about" class="section">
<h2>About Our Software</h2>
<p style="text-align:center; max-width:800px; margin:auto;">
Our Pharmacy Management System helps medical store owners manage billing, GST, stock, purchase, expiry alerts, customer credit and detailed reports easily.
Designed specially for Indian pharmacies.
</p>
</section>

<section id="features" class="section">
<h2>Key Features</h2>

<div class="features">
<div class="features">
    <div class="card"><h3>⚡ Fast Billing</h3><p>Generate invoices in seconds with shortcut support.</p></div>
    <div class="card"><h3>🧾 GST Ready</h3><p>Automatic GST, HSN codes, and GSTR reports.</p></div>
    <div class="card"><h3>📦 Stock Control</h3><p>Batch‑wise stock, expiry alerts, and low‑stock warnings.</p></div>
    <div class="card"><h3>🛒 Purchase Module</h3><p>Supplier bills, returns, and outstanding tracking.</p></div>
    <div class="card"><h3>👥 Customer Ledger</h3><p>Credit history, payments, and balance reports.</p></div>
    <div class="card"><h3>📊 Reports</h3><p>Sales, profit, tax, and monthly analysis reports.</p></div>
  </div>

</section>

<section id="pricing" class="section">
<h2>Pricing Plans</h2>
<div class="pricing">

<div class="price-card">
<h3>Premium</h3>
<div class="price">₹10,000</div>
<p>One-time payment For 5 Years</p>
<br>
<a href="https://wa.me/919412561200" target="_blank" class="btn">
    <i class="fa-brands fa-whatsapp"></i> Contact Now
</a>
</div>

<div class="price-card">
<h3>Basic</h3>
<div class="price">₹2499</div>
<p>With 1 Year Support</p>
<br>

<a href="https://wa.me/919412561200" target="_blank" class="btn">
    <i class="fa-brands fa-whatsapp"></i> Contact Now
</a>

</div>

</div>
</section>

<section id="contact" class="section contact">
<h2>Contact Us</h2>
<a href="tel:+919412561200">📞 +91 9412561200</a>
<a href="https://wa.me/919412561200?text=Hello%20I%20need%20pharmacy%20software" target="_blank">
<i class="fa-brands fa-whatsapp"></i> WhatsApp Support
</a>
</section>

<!-- WhatsApp Floating Button -->
<a href="https://wa.me/919412561200?text=Hello%20I%20need%20Pharmacy%20Software"
   target="_blank"
   class="float-whatsapp">

   <i class="fa-brands fa-whatsapp"></i>

</a>


<footer>

<p>© 2026 Pharmacy Management System | All Rights Reserved</p>
</footer>


