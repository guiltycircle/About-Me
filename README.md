<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alvin | About Me</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Montserrat:wght@700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #1a237e;
            --secondary: #3949ab;
            --accent: #00bcd4;
            --bg: #f5f7fa;
            --card-bg: #fff;
            --text: #222;
            --muted: #6c757d;
        }
        body {
            margin: 0;
            padding: 0;
            background: var(--bg);
            font-family: 'Roboto', sans-serif;
            color: var(--text);
        }
        .hero {
            background: linear-gradient(120deg, var(--primary) 60%, var(--accent) 100%);
            padding: 48px 0 80px 0;
            text-align: center;
            position: relative;
        }
        .brand {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            color: #fff;
            letter-spacing: 2px;
            font-weight: 700;
            margin-bottom: 8px;
            text-shadow: 0 2px 8px rgba(0,0,0,0.12);
        }
        .hero-desc {
            color: #e3e7fa;
            font-size: 1.2rem;
            margin-bottom: 0;
        }
        .profile-card {
            background: var(--card-bg);
            max-width: 420px;
            margin: -60px auto 0 auto;
            border-radius: 18px;
            box-shadow: 0 8px 32px rgba(26,35,126,0.10);
            padding: 36px 28px 28px 28px;
            position: relative;
            z-index: 2;
            animation: fadeInUp 1s cubic-bezier(.23,1.01,.32,1) 0.2s both;
        }
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .profile-photo {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: #e0e0e0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            color: #b0b0b0;
            margin: 0 auto 18px auto;
            box-shadow: 0 2px 12px rgba(0,0,0,0.07);
            transition: box-shadow 0.2s;
        }
        .profile-photo:hover {
            box-shadow: 0 4px 24px rgba(0,188,212,0.18);
        }
        h1 {
            text-align: center;
            margin: 0 0 8px 0;
            font-size: 2rem;
            font-family: 'Montserrat', sans-serif;
            color: var(--primary);
        }
        .bio {
            text-align: center;
            margin-bottom: 18px;
            color: var(--muted);
            font-size: 1.08rem;
        }
        .section {
            margin-bottom: 18px;
        }
        .section-title {
            font-weight: 700;
            margin-bottom: 6px;
            color: var(--secondary);
            font-size: 1.08rem;
            letter-spacing: 1px;
        }
        .hobbies {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            justify-content: flex-start;
        }
        .hobby {
            background: var(--accent);
            color: #fff;
            padding: 8px 20px;
            border-radius: 16px;
            font-size: 1rem;
            font-weight: 500;
            box-shadow: 0 1px 4px rgba(0,188,212,0.08);
            transition: background 0.2s;
            width: 80%;
            max-width: 260px;
            text-align: center;
        }
        .hobby:hover {
            background: var(--secondary);
        }
        .profession-list {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            margin-top: 8px;
        }
        .profession-item {
            background: #e3e7fa;
            color: var(--primary);
            padding: 8px 20px;
            border-radius: 16px;
            font-size: 1rem;
            font-weight: 500;
            width: 80%;
            max-width: 260px;
            text-align: center;
        }
        .social-links {
            display: flex;
            justify-content: center;
            gap: 28px;
            margin-top: 8px;
        }
        .social-links a {
            color: var(--secondary);
            text-decoration: none;
            font-size: 2rem;
            transition: color 0.2s, transform 0.2s;
            position: relative;
        }
        .social-links a:hover {
            color: var(--accent);
            transform: translateY(-3px) scale(1.08);
        }
        .social-links a::after {
            content: attr(data-tooltip);
            position: absolute;
            left: 50%;
            transform: translateX(-50%) scale(0.9);
            bottom: -28px;
            background: #222;
            color: #fff;
            font-size: 0.85rem;
            padding: 2px 10px;
            border-radius: 8px;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.2s, transform 0.2s;
            white-space: nowrap;
        }
        .social-links a:hover::after {
            opacity: 1;
            transform: translateX(-50%) scale(1);
        }
        @media (max-width: 600px) {
            .profile-card {
                padding: 18px 4px 18px 4px;
            }
            .hero {
                padding: 32px 0 60px 0;
            }
        }
    </style>
    <script src="https://kit.fontawesome.com/4b7e5e6e8b.js" crossorigin="anonymous"></script>
</head>
<body>
    <div class="hero">
        <div class="brand">Alvin</div>
        <div class="hero-desc">Official Portfolio &mdash; Computer Science Student & Programmer</div>
    </div>
    <div class="profile-card">
        <div class="profile-photo">
            <span><i class="fas fa-user"></i></span>
        </div>
        <h1>Alvin</h1>
        <div class="bio">
            I am a computer science student working at Zerxis Limited, a call center helpline. Passionate about programming and technology.
        </div>
        <div class="section">
            <div class="section-title">Profession</div>
            <div class="profession-list">
                <div class="profession-item">Programmer</div>
                <div class="profession-item">Computer Science Student</div>
                <div class="profession-item">Call Center Helpline (Zerxis Limited)</div>
            </div>
        </div>
        <div class="section">
            <div class="section-title">Hobbies & Interests</div>
            <div class="hobbies">
                <div class="hobby">Programming</div>
                <div class="hobby">Design</div>
                <div class="hobby">Mobile</div>
                <div class="hobby">Backend</div>
                <div class="hobby">Frontend</div>
            </div>
        </div>
        <div class="section">
            <div class="section-title">Connect with me</div>
            <div class="social-links">
                <a href="#" data-tooltip="Instagram" title="Instagram" target="_blank"><i class="fab fa-instagram"></i></a>
                <a href="#" data-tooltip="Twitter" title="Twitter" target="_blank"><i class="fab fa-twitter"></i></a>
                <a href="#" data-tooltip="GitHub" title="GitHub" target="_blank"><i class="fab fa-github"></i></a>
            </div>
        </div>
    </div>
</body>
</html> 
