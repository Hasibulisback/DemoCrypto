# DemoCrypto
Demo description
<!DOCTYPE html>
<html lang="bn">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Shiba Inu-এর মতো ওয়েবসাইট</title>
 <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
 <style>
 body {
 font-family: 'Poppins', sans-serif;
 margin: 0;
 padding: 0;
 box-sizing: border-box;
 background-color: #f4f7fa;
 color: #333;
 line-height: 1.6;
 }

 .container {
 max-width: 1200px;
 margin: 0 auto;
 padding: 20px;
 }

 /* Header */
 header {
 background-color: #fff;
 padding: 15px 0;
 box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
 position: sticky;
 top: 0;
 z-index: 1000;
 }

 nav {
 display: flex;
 justify-content: space-between;
 align-items: center;
 }

 .logo {
 font-size: 1.8em;
 font-weight: 700;
 color: #007bff;
 text-decoration: none;
 }

 .nav-links {
 list-style: none;
 margin: 0;
 padding: 0;
 display: flex;
 }

 .nav-links li {
 margin-left: 30px;
 }

 .nav-links a {
 text-decoration: none;
 color: #555;
 font-weight: 500;
 transition: color 0.3s ease;
 }

 .nav-links a:hover {
 color: #007bff;
 }

 /* Hero Section */
 #hero {
 background: linear-gradient(135deg, #007bff, #00c6ff);
 color: #fff;
 padding: 100px 0;
 text-align: center;
 display: flex;
 flex-direction: column;
 justify-content: center;
 align-items: center;
 min-height: 80vh;
 }

 #hero h1 {
 font-size: 3.5em;
 margin-bottom: 10px;
 font-weight: 700;
 }

 #hero p {
 font-size: 1.4em;
 margin-bottom: 30px;
 font-weight: 300;
 }

 .btn {
 background-color: #fff;
 color: #007bff;
 padding: 12px 25px;
 border-radius: 5px;
 text-decoration: none;
 font-weight: 600;
 transition: background-color 0.3s ease, color 0.3s ease;
 }

 .btn:hover {
 background-color: #e2e6ea;
 }

 /* Sections General */
 section {
 padding: 80px 0;
 text-align: center;
 }

 section:nth-child(even) {
 background-color: #e9f0f7;
 }

 h2 {
 font-size: 2.5em;
 margin-bottom: 40px;
 color: #007bff;
 position: relative;
 display: inline-block;
 }

 h2::after {
 content: '';
 width: 80px;
 height: 4px;
 background-color: #007bff;
 position: absolute;
 bottom: -10px;
 left: 50%;
 transform: translateX(-50%);
 border-radius: 2px;
 }

 /* About Section */
 #about .about-content {
 display: flex;
 flex-wrap: wrap;
 justify-content: center;
 align-items: center;
 gap: 40px;
 text-align: left;
 }

 #about .about-content img {
 max-width: 300px;
 border-radius: 8px;
 box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
 }

 #about .text-content {
 max-width: 600px;
 }

 /* Token Info Section */
 #token-info .token-grid {
 display: grid;
 grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
 gap: 30px;
 margin-top: 40px;
 }

 #token-info .token-card {
 background-color: #fff;
 border-radius: 8px;
 overflow: hidden;
 box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
 transition: transform 0.3s ease;
 text-align: left;
 padding: 20px;
 }

 #token-info .token-card:hover {
 transform: translateY(-5px);
 }

 #token-info .token-card h3 {
 font-size: 1.5em;
 margin-top: 0;
 color: #007bff;
 }

 #token-info .token-card p {
 font-size: 0.95em;
 color: #666;
 }

 /* Staking Section */
 #staking .staking-options {
 display: flex;
 justify-content: space-around;
 margin-top: 30px;
 }

 #staking .staking-option {
 background-color: #fff;
 padding: 20px;
 border-radius: 8px;
 box-shadow: 0 2px 5px rgba(0, 0, 0, 0.08);
 transition: transform 0.3s ease;
 }

 #staking .staking-option:hover {
 transform: translateY(-5px);
 }

 /* Community Section */
 #community .community-links {
 display: flex;
 justify-content: space-around;
 margin-top: 30px;
 }

 #community .community-link {
 background-color: #fff;
 padding: 20px;
 border-radius: 8px;
 box-shadow: 0 2px 5px rgba(0, 0, 0, 0.08);
 transition: transform 0.3s ease;
 }

 #community .community-link:hover {
 transform: translateY(-5px);
 }

 /* Contact Section */
 #contact .contact-form {
 max-width: 600px;
 margin: 0 auto;
 text-align: left;
 }

 #contact .form-group {
 margin-bottom: 20px;
 }

 #contact label {
 display: block;
 margin-bottom: 8px;
 font-weight: 600;
 }

 #contact input[type="text"],
 #contact input[type="email"],
 #contact textarea {
 width: 100%;
 padding: 12px;
 border: 1px solid #ccc;
 border-radius: 5px;
 font-size: 1em;
 box-sizing: border-box; /* Ensures padding doesn't increase width */
 }

 #contact textarea {
 resize: vertical;
 min-height: 120px;
 }

 #contact button[type="submit"] {
 background-color: #007bff;
 color: #fff;
 padding: 12px 30px;
 border: none;
 border-radius: 5px;
 cursor: pointer;
 font-size: 1.1em;
 font-weight: 600;
 transition: background-color 0.3s ease;
 }

 #contact button[type="submit"]:hover {
 background-color: #0056b3;
 }

 /* Footer */
 footer {
 background-color: #333;
 color: #fff;
 text-align: center;
 padding: 25px 0;
 margin-top: 50px;
 }

 footer p {
 margin: 0;
 font-size: 0.9em;
 }

 /* Responsive Design */
 @media (max-width: 768px) {
 .nav-links {
 display: none; /* Hide nav links on small screens for simplicity */
 }

 #hero h1 {
 font-size: 2.5em;
 }

 #hero p {
 font-size: 1.1em;
 }

 h2 {
 font-size: 2em;
 }

 #about .about-content {
 flex-direction: column;
 }

 #about .about-content img {
 max-width: 250px;
 }

 #token-info .token-grid,
 #projects .projects-grid {
 grid-template-columns: 1fr; /* Single column layout on small screens */
 }

 #staking .staking-options,
 #community .community-links {
 flex-direction: column;
 align-items: center;
 }

 #staking .staking-option,
 #community .community-link {
 margin-bottom: 20px;
 width: 80%;
 }
 }
 </style>
</head>
<body>

 <header>
 <div class="container">
 <nav>
 <a href="#" class="logo">Shiba Inu-এর মতো</a>
 <ul class="nav-links">
 <li><a href="#about">আমার সম্পর্কে</a></li>
 <li><a href="#token-info">টোকেন তথ্য</a></li>
 <li><a href="#staking">স্ট্যাকিং</a></li>
 <li><a href="#community">কমিউনিটি</a></li>
 <li><a href="#contact">যোগাযোগ</a></li>
 </ul>
 </nav>
 </div>
 </header>

 <section id="hero">
 <div class="container">
 <h1>Shiba Inu-এর মতো একটি ওয়েবসাইট</h1>
 <p>এটি একটি ডেমো ওয়েবসাইট, যেখানে Shiba Inu-এর মতো ক্রিপ্টোকারেন্সি সম্পর্কিত তথ্য দেওয়া হয়েছে।</p>
 <a href="#contact" class="btn">যোগাযোগ করুন</a>
 </div>
 </section>

 <section id="about">
 <div class="container">
 <h2>আমার সম্পর্কে</h2>
 <div class="about-content">
 <img src="http://googleusercontent.com/generated_image_content/0" alt="ক্রিপ্টোকারেন্সি ওয়েবসাইট">
 <div class="text-content">
 <p>এই ওয়েবসাইটটি Shiba Inu দ্বারা অনুপ্রাণিত। এখানে ক্রিপ্টোকারেন্সি, স্ট্যাকিং এবং কমিউনিটি সম্পর্কিত তথ্য রয়েছে।</p>
 </div>
 </div>
 </div>
 </section>

 <section id="token-info">
 <div class="container">
 <h2>টোকেন তথ্য</h2>
 <div class="token-grid">
 <div class="token-card">
 <h3>SHIB</h3>
 <p>Shiba Inu (SHIB) একটি বিকেন্দ্রীভূত ক্রিপ্টোকারেন্সি।</p>
 </div>
 <div class="token-card">
 <h3>BONE</h3>
 <p>BONE হলো ইকোসিস্টেমের গভর্নেন্স টোকেন।</p>
 </div>
 <div class="token-card">
 <h3>LEASH</h3>
 <p>LEASH টোকেনটি ইকোসিস্টেমের অনুগতদের জন্য বিশেষভাবে তৈরি।</p>
 </div>
 </div>
 </div>
 </section>

 <section id="staking">
 <div class="container">
 <h2>স্ট্যাকিং</h2>
 <p>এখানে স্ট্যাকিং এর বিভিন্ন অপশন এবং সুবিধা সম্পর্কে জানতে পারবেন।</p>
 <div class="staking-options">
 <div class="staking-option">স্ট্যাকিং অপশন ১</div>
 <div class="staking-option">স্ট্যাকিং অপশন ২</div>
 </div>
 </div>
 </section>

 <section id="community">
 <div class="container">
 <h2>কমিউনিটি</h2>
 <p>Shiba Inu কমিউনিটির বিভিন্ন মাধ্যম এবং কার্যকলাপ সম্পর্কে জানুন।</p>
 <div class="community-links">
 <div class="community-link">টেলিগ্রাম</div>
 <div class="community-link">ডিসকর্ড</div>
 </div>
 </div>
 </section>

 <section id="contact">
 <div class="container">
 <h2>যোগাযোগ করুন</h2>
 <form class="contact-form" action="#" method="POST">
 <div class="form-group">
 <label for="name">আপনার নাম:</label>
 <input type="text" id="name" name="name" required>
 </div>
 <div class="form-group">
 <label for="email">আপনার ইমেল:</label>
 <input type="email" id="email" name="email" required>
 </div>
 <div class="form-group">
 <label for="message">আপনার বার্তা:</label>
 <textarea id="message" name="message" required></textarea>
 </div>
 <button type="submit">বার্তা পাঠান</button>
 </form>
 </div>
 </section>

 <footer>
 <div class="container">
 <p>&copy; 2025 Shiba Inu-এর মতো। সর্বস্বত্ব সংরক্ষিত।</p>
 </div>
 </footer>

</body>
</html>
