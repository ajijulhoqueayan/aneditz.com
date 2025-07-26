<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>AnEditz | Logo Shop</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f8f8f8;
      color: #333;
    }
    header {
      background: #111;
      color: #fff;
      padding: 20px;
      text-align: center;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      padding: 20px;
    }
    .gallery img {
      width: 100%;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .contact, .order-form {
      background: #fff;
      padding: 20px;
      margin: 10px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    .contact h2, .order-form h2 {
      text-align: center;
    }
    .contact p, .order-form label {
      font-size: 16px;
      margin: 8px 0;
    }
    .order-form input, .order-form textarea {
      width: 100%;
      padding: 8px;
      margin-bottom: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    .order-form button {
      padding: 10px 20px;
      background: #111;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      background: #111;
      color: #fff;
      text-align: center;
      padding: 10px;
      font-size: 14px;
    }
    .whatsapp {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #25D366;
      color: white;
      border-radius: 50%;
      width: 55px;
      height: 55px;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 30px;
      text-decoration: none;
    }
    .admin-panel {
      text-align: center;
      margin: 20px;
    }
    .admin-panel input[type="password"] {
      padding: 8px;
      width: 200px;
      margin: 10px;
    }
    .admin-panel button {
      padding: 8px 15px;
      background-color: #222;
      color: #fff;
      border: none;
      border-radius: 5px;
    }
    #admin-content {
      display: none;
      padding: 20px;
      background: #fff3e6;
      margin: 10px;
      border-radius: 10px;
    }
  </style>
</head>
<body>

<header>
  <h1>Welcome to AnEditz Logo Store</h1>
  <p>Buy Creative Logos or Contact for Custom Design</p>
</header>

<section class="gallery">
  <img src="logo1.jpg" alt="Logo 1">
  <img src="logo2.jpg" alt="Logo 2">
  <img src="logo3.jpg" alt="Logo 3">
</section>

<section class="order-form">
  <h2>অর্ডার করুন</h2>
  <form>
    <label>আপনার নাম:</label>
    <input type="text" placeholder="আপনার নাম লিখুন" required>
    
    <label>আপনার ইমেইল:</label>
    <input type="email" placeholder="ইমেইল লিখুন" required>
    
    <label>অর্ডার বিবরণ:</label>
    <textarea rows="4" placeholder="আপনার প্রয়োজন লিখুন" required></textarea>
    
    <button type="submit">সাবমিট করুন</button>
  </form>
</section>

<section class="contact">
  <h2>যোগাযোগ করুন</h2>
  <p>📞 মোবাইল: <a href="tel:01646364595">01646364595</a></p>
  <p>📧 ইমেইল: <a href="mailto:ajijulhoqueayan50@gmail.com">ajijulhoqueayan50@gmail.com</a></p>
</section>

<section class="admin-panel">
  <h2>🔒 Super Admin Panel</h2>
  <input type="password" id="adminPassword" placeholder="Enter password">
  <button onclick="checkAdmin()">Log In</button>
</section>

<div id="admin-content">
  <h3>🎨 Add New Logo (এখানে কোডে লোগো এড করতে হবে)</h3>
  <p>নতুন লোগো এড করতে <code>&lt;img src="newlogo.jpg"&gt;</code> এই ফরম্যাট ব্যবহার করুন।</p>
</div>

<a href="https://wa.me/8801646364595" class="whatsapp" target="_blank" title="WhatsApp"><b>💬</b></a>

<footer>
  &copy; 2025 AnEditz.com | All rights reserved.
</footer>

<script>
  function checkAdmin() {
    var password = document.getElementById("adminPassword").value;
    if (password === "an041212") {
      document.getElementById("admin-content").style.display = "block";
      alert("Welcome, Admin!");
    } else {
      alert("Incorrect password!");
    }
  }
</script>

</body>
</html>
