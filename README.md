<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <a href="https://github.com/hayomi123/jadid.git"></a>
    <title>Selamat Ulang Tahun!</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@400;700&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
        a

        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            overflow: hidden;
            height: 100vh;
            width: 100vw;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            background: linear-gradient(45deg, #f2e6d9, #f9f9f9); /* Gradasi cream redup */
            animation: backgroundShift 200s infinite alternate;
        }

        @keyframes backgroundShift {
            0% { background: linear-gradient(45deg, #f2e6d9, #f9f9f9); }
            50% { background: linear-gradient(45deg, #e8d5e8, #f9f9f9); }
            100% { background: linear-gradient(45deg, #f2e6d9, #f9f9f9); }
        }

        .content {
            position: relative;
            z-index: 2;
            text-align: center;
            padding: 20px;
            background: rgba(255, 255, 255, 0.85); /* Latar belakang putih semi-transparan */
            border-radius: 20px;
            box-shadow: 0 0 30px rgba(0, 0, 0, 0.4);
            width: 90%;
            max-width: 800px;
            max-height: 85vh;
            overflow: hidden;
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            color: #ff6f61;
            text-shadow: 0 0 15px rgba(255, 105, 100, 100);
            font-size: 3.5em;
            margin-bottom: 20px;
            animation: fadeInUp 3s ease-out;
        }

        .message-container {
            position: relative;
            overflow: hidden;
            height: 400px; /* Height for scrolling */
            width: 100%;
            display: none; /* Initially hidden */
        }

        .scrolling-text {
            position: absolute;
            bottom: 0;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            animation: slideUp 30s ease-in-out infinite, fadeInOutText 100s infinite;
        }

        .scrolling-text p {
            margin: 0;
            font-size: 1.4em;
            line-height: 1.8;
            padding: 15px 0;
            white-space: nowrap;
            color: #333; /* Warna teks lebih gelap */
        }

        @keyframes fadeInUp {
            0% { opacity: 0; transform: translateY(20px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideUp {
            0% { transform: translateY(100%); }
            100% { transform: translateY(-100%); }
        }

        @keyframes fadeInOutText {
            0%, 100% { opacity: 0; }
            5%, 25% { opacity: 1; }
        }

        /* Bintang */
        .star {
            position: absolute;
            width: 50px;
            height: 50px;
            background: url('https://www.w3schools.com/w3images/star.png') no-repeat center center;
            background-size: contain;
            z-index: 1;
            opacity: 0.9;
            animation: twinkle 210s infinite alternate;
        }

        .star.top-left {
            top: 20px;
            left: 20px;
        }

        .star.top-right {
            top: 20px;
            right: 20px;
        }

        .star.bottom-left {
            bottom: 20px;
            left: 20px;
        }

        .star.bottom-right {
            bottom: 20px;
            right: 20px;
        }

        /* Partikel Salju */
        .snowflake {
            position: absolute;
            color: #fff;
            font-size: 1.8em;
            user-select: none;
            pointer-events: none;
            animation: fall 25s linear infinite;
            opacity: 6;
        }

        @keyframes fall {
            0% { transform: translateY(-100vh) rotate(0deg); }
            100% { transform: translateY(100vh) rotate(360deg); }
        }

        /* Kue Ulang Tahun */
        .cake {
            margin: 20px 0;
            width: 200px;
            height: auto;
            background: url('https://www.w3schools.com/w3images/cake.jpg') no-repeat center center;
            background-size: cover;
            position: relative;
            animation: fireworks 2s ease-out;
        }

        @keyframes fireworks {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.1); opacity: 0.7; }
            100% { transform: scale(1); opacity: 1; }
        }

        /* Tombol */
        .reveal-button {
            margin-top: 20px;
            padding: 12px 25px;
            font-size: 1.4em;
            color: #fff;
            background-color: #ff6f61;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            transition: background-color 5s ease;
        }0.3s

        .reveal-button:hover {
            background-color: #ff5a4f;
        }

        @keyframes fadeInButton {
            0% { opacity: 0; transform: translateY(20px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        /* Media Queries */
        @media (max-width: 768px) {
            h1 {
                font-size: 3em;
            }

            .message-container {
                height: 300px;
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 2.5em;
            }

            .message-container {
                height: 250px;
                font-size: 1em;
            }

            .cake {
                width: 150px;
            }
        }

    </style>
</head>
<body>
    <div class="content">
        <h1>Happy Birthday My Girlfriend</h1>
        <div class="cake"></div>

        <button class="reveal-button" onclick="revealMessage()">Klik Di Sini</button>
        <div class="message-container">
            <div class="scrolling-text">
                <p>Semoga hari ini penuh dengan kebahagiaan dan cinta.</p>

                <br><br><br>
                <p>Di setiap langkah yang kamu ambil, semoga keberuntungan selalu menyertaimu.</p>
                <p>Semoga segala rintangan menjadi pelajaran dan pengalaman yang berharga.</p>
                <p>Di tahun yang baru ini, semoga semua impianmu tercapai, dan kamu terus berkembang menjadi pribadi yang lebih baik.</p>
                <p>Selamat merayakan hari istimewa ini, dan semoga tahun ini menjadi tahun terbaik dalam hidupmu!</p>
                <p>Kami semua berdoa agar hari-harimu dipenuhi dengan kebahagiaan dan kesuksesan.</p>
                <p>Jangan lupa untuk terus mengejar impianmu dan tetap semangat!</p>
                <p>Semoga setiap tahun membawa kebahagiaan yang lebih besar daripada tahun sebelumnya.</p>
                <p>Terima kasih telah menjadi inspirasi bagi kami semua!</p>
                <p>Selamat Ulang Tahun sekali lagi dan semoga segala yang terbaik selalu menyertaimu!</p>
            </div>
        </div>
        <!-- Elemen Bintang -->
        <div class="star top-left"></div>
        <div class="star top-right"></div>
        <div class="star bottom-left"></div>
        <div class="star bottom-right"></div>
        <!-- Elemen Salju -->
        <div id="snowflakes"></div>
    </div>

    <script>
        // Partikel Salju
        function createSnowflake() {
            const snowflake = document.createElement('div');
            snowflake.className = 'snowflake';
            snowflake.textContent = '❄';
            snowflake.style.left = Math.random() * 100 + 'vw';
            snowflake.style.fontSize = Math.random() * 15 + 15 + 'px';
            snowflake.style.animationDuration = Math.random() * 5 + 7 + 's';
            snowflake.style.transform = 'rotate(' + Math.random() * 360 + 'deg)';
            document.getElementById('snowflakes').appendChild(snowflake);
        }

        for (let i = 0; i < 60; i++) {
            createSnowflake();
        }

        function revealMessage() {
            document.querySelector('.message-container').style.display = 'block';
            document.querySelector('.reveal-button').style.display = 'none';
        }
    </script>
</body>
</html>
