<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shiba Inu-এর মতো ওয়েবসাইট</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
        }
        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            display: block;
        }
        nav a:hover {
            background-color: #2c3e50;
        }
        .hero {
            background-color: #e67e22;
            color: white;
            padding: 60px 20px;
            text-align: center;
        }
        .about {
            padding: 40px 20px;
            text-align: center;
            background-color: white;
        }
        .about img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
        }
        .contact {
            padding: 40px 20px;
            text-align: center;
            background-color: #ecf0f1;
        }
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px;
        }
        form {
            max-width: 400px;
            margin: 0 auto;
        }
        input, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
            margin-bottom: 20px;
            border: 1px solid #bdc3c7;
            border-radius: 5px;
        }
        button {
            background-color: #e67e22;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #d35400;
        }
    </style>
</head>
<body>
    <header>
        <h1>Shiba Inu ওয়েবসাইটে আপনাকে স্বাগতম</h1>
    </header>
    <nav>
        <a href="#home">মূলপাতা</a>
        <a href="#about">আমাদের সম্পর্কে</a>
        <a href="#contact">যোগাযোগ</a>
    </nav>
    <section class="hero" id="home">
        <h2>আমরা ক্রিপ্টোকারেন্সির ভবিষ্যৎ গড়ছি</h2>
        <p>Shiba Inu-এর মতো শক্তিশালী ও নিরাপদ প্ল্যাটফর্ম তৈরি করুন</p>
    </section>
    <section class="about" id="about">
        <h2>আমাদের সম্পর্কে</h2>
        <p>আমরা একটি উদ্ভাবনী দল যারা ব্লকচেইন প্রযুক্তি ব্যবহার করে নিরাপদ ও বিশ্বাসযোগ্য ক্রিপ্টো প্ল্যাটফর্ম তৈরি করি।</p>
        <img src="https://via.placeholder.com/300x200" alt="ক্রিপ্টোকারেন্সি সম্পর্কিত চিত্র">
    </section>
    <section class="contact" id="contact">
        <h2>যোগাযোগ করুন</h2>
        <form action="#">
            <label for="name">নাম:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">ইমেইল:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">বার্তা:</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <button type="submit">পাঠান</button>
        </form>
    </section>
    <footer>
        <p>&copy; ২০২৫ Shiba Inu ওয়েবসাইট. সর্বস্বত্ব সংরক্ষিত।</p>
    </footer>
</body>
</html>
