<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem Loading...</title>
    <style>
        *, *::before, *::after {
            box-sizing: border-box;
        }

        body {
            background-color: #000000; /* Hitam pekat kosong sepenuhnya */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            overflow: hidden;
            font-family: Arial, sans-serif;
        }

        /* Skrin 1: Intro Klik Heart */
        #intro-screen {
            text-align: center;
            cursor: pointer;
            z-index: 20;
        }
        .heart-emoji {
            font-size: 80px;
            margin-bottom: 10px;
            animation: slowPulse 2s infinite ease-in-out;
        }
        .click-text {
            color: #ffffff;
            font-size: 16px;
            font-weight: bold;
            letter-spacing: 1px;
        }
        @keyframes slowPulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        /* Skrin 2: Kandungan Utama */
        #main-screen {
            display: none;
            text-align: center;
            z-index: 10;
            width: 100%;
        }

        /* HATI SAIZ SEDERHANA (NGAM UNTUK PFP) */
        .heart-text-container {
            font-family: 'Times New Roman', Times, serif; 
            color: #ff0000; /* Merah terang menyala asli */
            font-size: 14px; /* Ditukar ke 14px untuk saiz sederhana ideal */
            font-weight: bold;
            line-height: 1.3; /* Jarak baris yang mampat dan kemas */
            letter-spacing: 2px;
            display: inline-block;
            animation: heartbeat 1.2s infinite ease-in-out;
            filter: drop-shadow(0 0 12px rgba(255, 0, 0, 0.85)); /* Glow merah ngam-ngam */
        }

        .line {
            display: block;
            text-align: center;
            white-space: pre;
        }

        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.04); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>

    <div id="intro-screen" onclick="bukaKejutan()">
        <div class="heart-emoji">❤️</div>
        <div class="click-text">klik heart</div>
    </div>

    <div id="main-screen">
        <div class="heart-text-container">
            <span class="line">dayahdayah         dayahdayah</span>
            <span class="line">dayahdayahdayah     dayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayahdayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayahdayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayahdayah</span>
            <span class="line">dayahdayahdayah</span>
            <span class="line">dayahdayah</span>
            <span class="line">dayah</span>
        </div>
    </div>

    <script>
        function bukaKejutan() {
            document.getElementById('intro-screen').style.display = 'none';
            document.getElementById('main-screen').style.display = 'block';
        }
    </script>

</body>
</html>
