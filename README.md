<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To Mommy G</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: radial-gradient(circle, #ff9a9e 0%, #fecfef 100%);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            text-align: center;
        }

        /* Floating Hearts Background Animation */
        .heart {
            position: absolute;
            color: rgba(255, 255, 255, 0.6);
            font-size: 20px;
            user-select: none;
            animation: float 10s linear infinite;
            z-index: 1;
        }

        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-10vh) rotate(360deg); opacity: 0; }
        }

        .container {
            background: rgba(255, 255, 255, 0.9);
            padding: 40px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            max-width: 500px;
            width: 90%;
            z-index: 10;
            border: 2px solid #ff758c;
            animation: fadeIn 2s ease-in-out;
        }

        h1 { color: #ff758c; font-size: 2rem; margin-bottom: 20px; }
        
        .message {
            color: #555;
            line-height: 1.8;
            font-size: 1.2rem;
            font-style: italic;
            margin-bottom: 30px;
        }

        .signature {
            font-weight: bold;
            color: #ff758c;
            font-size: 1.3rem;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }
    </style>
</head>
<body>

    <script>
        for (let i = 0; i < 15; i++) {
            let heart = document.createElement('div');
            heart.className = 'heart';
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDelay = Math.random() * 10 + 's';
            heart.style.fontSize = (Math.random() * 20 + 10) + 'px';
            document.body.appendChild(heart);
        }
    </script>

    <div class="container">
        <h1>To: Mommy G ❤️</h1>
        <div class="message">
            Mommy, thank you for being my mom. I will miss you a lot. <br><br>
            When I miss my mama, I can hug you... but now, asa naman ko ani? <br><br>
            I miss you and wish you all the best. Amping mommy.
        </div>
        <div class="signature">I Love You!</div>
    </div>

</body>
</html>
