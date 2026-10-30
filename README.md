<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>My Pharmacy - Inventory Management System</title>
<!-- Bootstrap 5 CSS CDN -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
<!-- Font Awesome for Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
/* CUSTOM STYLING OVERRIDES & ENHANCEMENTS */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: #f6f9fb;
  color: #333;
}

/* HERO HEADER WITH CURVE */
header {
  position: relative;
  background: linear-gradient(135deg, #0b6e4f, #1bb98a);
  color: #fff;
  padding: 80px 20px 120px 20px;
  text-align: center;
  overflow: hidden;
}

header::after {
  content: "";
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  height: 80px;
  background: #f6f9fb;
  border-top-left-radius: 100% 80px;
  border-top-right-radius: 100% 80px;
}

/* RGB animation */
@keyframes rgbColor {
  0% { color: #ff4d4d; }
  33% { color: #4da6ff; }
  66% { color: #4dff88; }
  100% { color: #ff4d4d; }
}
.rgb-text {
  display: block;
  font-size: 42px;
  font-weight: 800;
  animation: rgbColor 4s infinite;
  margin-bottom: 10px;
}

/* CARDS */
.custom-card {
  position: relative;
  background: #fff;
  border-top: 5px solid #0b6e4f;
  padding: 25px;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  transition: 0.3s;
  height: 100%;
}

.custom-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 12px 25px rgba(0,0,0,0.15);
}

.custom-card h3 {
  color: #0b6e4f;
  font-size: 20px;
  margin-bottom: 15px;
  display: flex;
  align-items: center;
  gap: 10px;
}

/* BUTTON */
.btn-custom {
  display: inline-block;
  background: linear-gradient(135deg, #0b6e4f, #1bb98a);
  color: white;
  padding: 12px 24px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
  transition: 0.3s;
  border: none;
  cursor: pointer;
}

.btn-custom:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 18px rgba(0,0,0,0.2);
  color: white;
}

/* PRICING */
.price-card {
  background: white;
  padding: 40px;
  border-radius: 15px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  text-align: center;
  border: 1px solid #eee;
  position: relative;
  height: 100%;
}

.price-card.premium {
  border: 2px solid #1bb98a;
  transform: scale(1.03);
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
  text-decoration: none;
}

.float-whatsapp:hover {
  background-color: #20b557;
  transform: scale(1.1);
  color: white;
}

/* FOOTER */
footer {
  background: #064d38;
  color: #fff;
  text-align: center;
  padding: 30px;
  margin-top: 50px;
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
  <div class="container">
    <span class="rgb-text">My Pharmacy</span>
    <h1 class="display-5 fw-bold">Inventory Management System</h1>
    <p class="lead">All-in-one billing, GST & inventory software made for medical stores</p>
    <div class="mt-4">
      <a href="#download" class="btn btn-light text-success fw-bold px-4 py-2 shadow">Download Demo</a>
    </div>
  </div>
</header>

<!-- NAVBAR -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top" style="background-color: #064d38 !important;">
  <div class="container">
    <a class="navbar-brand fw-bold" href="#">My Pharmacy</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
      <div class="navbar-nav align-items-lg-center gap-3">
        <a class="nav-link text-white" href="#" onclick="alert('Contact Number: +91-9412561200')">Contact Us</a>
        <a class="nav-link text-white" href="tel:+919412561200">📞 +91 9412561200</a>
        <a class="nav-link text-success fw-semibold d-flex align-items-center gap-1" href="https://wa.me/919412561200?text=Hello%20I%20need%20support" target="_blank">
          <i class="fab fa-whatsapp fs-5"></i> WhatsApp
        </a>
      </div>
    </div>
  </div>
</nav>

<!-- KEY FEATURES -->
<section class="container py-5">
  <h2 class="text-center fw-bold mb-4" style="color: #0b6e4f;">Key Features</h2>
  <div class="row g-4">
    <div class="col-md-4">
      <div class="custom-card">
        <h3>⚡ Fast Billing</h3>
        <p>Generate invoices in seconds with shortcut support.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>🧾 GST Ready</h3>
        <p>Automatic GST, HSN codes, and GSTR reports.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>📦 Stock Control</h3>
        <p>Batch wise stock, expiry alerts, and low-stock warnings.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>🛒 Purchase Module</h3>
        <p>Supplier bills, returns, and outstanding tracking.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>👥 Customer Ledger</h3>
        <p>Credit history, payments, and balance reports.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>📊 Reports</h3>
        <p>Sales, profit, tax, and monthly analysis reports.</p>
      </div>
    </div>
  </div>
</section>

<!-- DOWNLOAD SECTION -->
<div id="download" class="text-center my-5">
  <a href="https://drive.google.com/uc?export=download&id=1NaMYOnSuCPI3HLGxhBHzctPTVF9Tvle0" class="btn-custom btn-lg" target="_blank">⬇ Download Free Demo</a>
</div>

<!-- PRICING PLANS -->
<section class="container py-5">
  <h2 class="text-center fw-bold mb-4" style="color: #0b6e4f;">Pricing Plans</h2>
  <div class="row justify-content-center g-4">
    <!-- Basic Plan -->
    <div class="col-md-4">
      <div class="price-card">
        <h3>Basic</h3>
        <div class="price">₹2,499</div>
        <p>With 1 Year Support</p>
        <ul>
          <li><i class="fas fa-check"></i> Billing Software</li>
          <li><i class="fas fa-check"></i> GST Reports</li>
          <li><i class="fas fa-check"></i> Stock Management</li>
          <li><i class="fas fa-times text-muted"></i> Advanced Analytics</li>
        </ul>
        <a href="https://wa.me/919412561200" target="_blank" class="btn-custom w-100">Contact Now</a>
      </div>
    </div>
  </div>
</section>

<!-- WHY CHOOSE US -->
<section class="container py-5">
  <h2 class="text-center fw-bold mb-4" style="color: #0b6e4f;">Why Choose Us?</h2>
  <div class="row g-4">
    <div class="col-md-4">
      <div class="custom-card">
        <h3>✔ Easy to Use</h3>
        <p>No training required. Simple interface for fast billing.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>✔ Affordable</h3>
        <p>Flexible one-time pricing with no hidden fees.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>✔ Trusted Support</h3>
        <p>Dedicated Phone & WhatsApp support.</p>
      </div>
    </div>
  </div>
</section>

<!-- BEST WISHES -->
<section class="container py-5">
  <h2 class="text-center fw-bold mb-4" style="color: #0b6e4f;">Best Wishes from My Pharmacy</h2>
  <div class="row g-4">
    <div class="col-md-4">
      <div class="custom-card">
        <h3>🚀 Grow With Confidence</h3>
        <p>We wish your pharmacy steady growth, smooth billing, and zero stress operations.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>🤝 Long-Term Partnership</h3>
        <p>Our goal is not just software, but a trusted relationship with every retailer.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>💊 Built for Indian Pharmacies</h3>
        <p>Designed keeping real medical store needs in mind.</p>
      </div>
    </div>
  </div>
</section>

<!-- PARTY MANAGEMENT SECTION -->
<section class="container py-5">
  <h2 class="text-center fw-bold mb-4" style="color: #0b6e4f;">Party / Supplier Management</h2>
  <div class="row g-4">
    <div class="col-md-4">
      <div class="custom-card">
        <h3>🏢 Party Master</h3>
        <p>Add & manage party details including Name, Address & Contact Number.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>📞 Contact Details</h3>
        <p>Store mobile number, GST number, and city information.</p>
      </div>
    </div>
    <div class="col-md-4">
      <div class="custom-card">
        <h3>💰 Outstanding Tracking</h3>
        <p>Track pending payments, credit balance & transaction history.</p>
      </div>
    </div>
  </div>

  <!-- Sample Party Table -->
  <div class="table-responsive mt-5">
    <table class="table table-striped table-bordered shadow-sm bg-white rounded overflow-hidden">
      <thead style="background:#0b6e4f; color:white;">
        <tr>
          <th>Party Name</th>
          <th>Contact</th>
          <th>GSTIN</th>
          <th>City</th>
          <th>Balance</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Shreeji Pharma Distributors</td>
          <td>+91 9876543210</td>
          <td>09AAAAA0000A1Z5</td>
          <td>Agra</td>
          <td>₹12,450 (Dr)</td>
        </tr>
        <tr>
          <td>Medica Healthcare</td>
          <td>+91 9123456789</td>
          <td>09BBBBB1111B1Z6</td>
          <td>Delhi</td>
          <td>₹0.00</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<!-- FLOATING WHATSAPP BUTTON -->
<a href="https://wa.me/919412561200?text=Hello%20I%20need%20Pharmacy%20Software" target="_blank" class="float-whatsapp">
  <i class="fab fa-whatsapp"></i>
</a>

<!-- FOOTER -->
<footer>
  <div class="container">
    <p class="mb-1">Trusted billing, GST & inventory software for modern Retailers</p>
    <p class="mb-0">&copy; 2026 My Pharmacy Inventory Management System | All Rights Reserved</p>
  </div>
</footer>

<!-- Bootstrap 5 JS Bundle CDN -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

