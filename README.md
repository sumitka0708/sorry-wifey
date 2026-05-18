[sorry-wifey.html](https://github.com/user-attachments/files/27963765/sorry-wifey.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>💕 Sorry Baby mera pyara baacha 💕</title>
    <style>
        /* ===== RESET & BASE ===== */
        *,
        *::before,
        *::after {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Poppins', cursive, sans-serif;
            min-height: 100vh;
            background: linear-gradient(135deg, #1a001a, #2d002d, #1a0030);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* ===== NAVIGATION BAR ===== */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            background: rgba(255, 192, 203, 0.15);
            backdrop-filter: blur(12px);
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid rgba(255, 105, 180, 0.3);
            box-shadow: 0 4px 30px rgba(255, 20, 147, 0.2);
        }

        .navbar .logo {
            font-size: 22px;
            font-weight: bold;
            color: #ff99cc;
            text-shadow: 0 0 20px #ff1493;
        }

        .navbar .nav-links {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
        }

        .navbar .nav-links a {
            color: #ffb6c1;
            text-decoration: none;
            font-size: 14px;
            font-weight: 600;
            padding: 6px 14px;
            border-radius: 50px;
            background: rgba(255, 20, 147, 0.15);
            border: 1px solid rgba(255, 105, 180, 0.3);
            transition: 0.3s;
        }

        .navbar .nav-links a:hover,
        .navbar .nav-links a.active {
            background: rgba(255, 20, 147, 0.4);
            border-color: #ff69b4;
            box-shadow: 0 0 20px rgba(255, 20, 147, 0.4);
            transform: scale(1.05);
        }

        /* ===== PAGE SECTIONS ===== */
        .page {
            display: none;
            min-height: 100vh;
            padding: 90px 20px 40px;
            animation: fadeInPage 0.6s ease;
        }

        .page.active {
            display: block;
        }

        @keyframes fadeInPage {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* ===== FLOATING HEARTS (background) ===== */
        .hearts-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
        }

        .heart-float {
            position: absolute;
            font-size: 20px;
            animation: floatUp linear infinite;
            opacity: 0.4;
        }

        @keyframes floatUp {
            0% {
                transform: translateY(100vh) rotate(0deg) scale(0.5);
                opacity: 0;
            }
            10% {
                opacity: 0.6;
            }
            90% {
                opacity: 0.6;
            }
            100% {
                transform: translateY(-10vh) rotate(720deg) scale(1.2);
                opacity: 0;
            }
        }

        /* ===== PAGE 1: LANDING / APOLOGY ===== */
        .landing {
            position: relative;
            z-index: 1;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 85vh;
        }

        .landing h1 {
            font-size: 3.5rem;
            color: #ffb6c1;
            text-shadow: 0 0 40px rgba(255, 20, 147, 0.6), 0 0 80px rgba(255, 105, 180, 0.3);
            animation: pulseGlow 2s ease-in-out infinite;
            margin-bottom: 10px;
        }

        @keyframes pulseGlow {
            0%,
            100% {
                text-shadow: 0 0 40px rgba(255, 20, 147, 0.6);
            }
            50% {
                text-shadow: 0 0 80px rgba(255, 20, 147, 0.9), 0 0 120px rgba(255, 105, 180, 0.5);
            }
        }

        .landing .subtitle {
            font-size: 1.3rem;
            color: #ff99cc;
            margin-bottom: 25px;
            font-style: italic;
        }

        .landing .big-heart {
            font-size: 120px;
            animation: heartbeat 1.2s ease-in-out infinite;
            display: inline-block;
            cursor: pointer;
            margin: 15px 0;
        }

        @keyframes heartbeat {
            0%,
            100% {
                transform: scale(1);
            }
            14% {
                transform: scale(1.3);
            }
            28% {
                transform: scale(1);
            }
            42% {
                transform: scale(1.3);
            }
            70% {
                transform: scale(1);
            }
        }

        .landing .sorry-msg {
            background: rgba(255, 182, 193, 0.1);
            border: 2px solid rgba(255, 105, 180, 0.3);
            border-radius: 30px;
            padding: 25px 40px;
            max-width: 600px;
            margin: 20px auto;
            backdrop-filter: blur(10px);
        }

        .landing .sorry-msg p {
            color: #ffc0cb;
            font-size: 1.2rem;
            line-height: 1.8;
        }

        .landing .sorry-msg .highlight {
            color: #ff69b4;
            font-weight: bold;
            font-size: 1.4rem;
        }

        /* ===== BUTTONS ===== */
        .btn {
            display: inline-block;
            padding: 14px 40px;
            margin: 10px;
            border: none;
            border-radius: 50px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.4s;
            text-decoration: none;
            color: #fff;
            background: linear-gradient(135deg, #ff1493, #ff69b4);
            box-shadow: 0 4px 25px rgba(255, 20, 147, 0.4);
        }

        .btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 8px 40px rgba(255, 20, 147, 0.6);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid #ff69b4;
            color: #ff69b4;
        }

        .btn-outline:hover {
            background: rgba(255, 105, 180, 0.2);
        }

        /* ===== PAGE 2: PANDA KISS PAGE ===== */
        .panda-page {
            position: relative;
            z-index: 1;
            text-align: center;
            padding-top: 30px;
        }

        .panda-page h2 {
            font-size: 2.8rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
            margin-bottom: 10px;
        }

        .panda-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 25px;
            margin-top: 20px;
        }

        .panda-container img {
            max-width: 350px;
            border-radius: 30px;
            box-shadow: 0 0 50px rgba(255, 105, 180, 0.3), 0 0 100px rgba(255, 20, 147, 0.15);
            border: 4px solid rgba(255, 105, 180, 0.3);
            animation: pandaBounce 2s ease-in-out infinite;
        }

        @keyframes pandaBounce {
            0%,
            100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-15px);
            }
        }

        .panda-container .panda-caption {
            color: #ffc0cb;
            font-size: 1.5rem;
            font-weight: 600;
            animation: blinkText 1.5s ease-in-out infinite;
        }

        @keyframes blinkText {
            0%,
            100% {
                opacity: 1;
            }
            50% {
                opacity: 0.5;
            }
        }

        .panda-kisses {
            font-size: 3rem;
            letter-spacing: 10px;
            animation: kissFloat 2s ease-in-out infinite;
        }

        @keyframes kissFloat {
            0%,
            100% {
                transform: translateY(0) rotate(0deg);
            }
            25% {
                transform: translateY(-10px) rotate(-5deg);
            }
            75% {
                transform: translateY(-10px) rotate(5deg);
            }
        }

        /* ===== PAGE 3: TIC TAC TOE ===== */
        .game-page {
            position: relative;
            z-index: 1;
            text-align: center;
        }

        .game-page h2 {
            font-size: 2.5rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
            margin-bottom: 10px;
        }

        .game-page .game-subtitle {
            color: #ff99cc;
            font-size: 1.1rem;
            margin-bottom: 20px;
        }

        .game-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }

        .game-board {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 8px;
            width: 330px;
            height: 330px;
            background: rgba(255, 182, 193, 0.08);
            border-radius: 20px;
            padding: 12px;
            border: 2px solid rgba(255, 105, 180, 0.25);
            box-shadow: 0 0 40px rgba(255, 20, 147, 0.15);
        }

        .cell {
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 192, 203, 0.08);
            border-radius: 12px;
            font-size: 3rem;
            font-weight: bold;
            color: #ffb6c1;
            cursor: pointer;
            transition: 0.25s;
            aspect-ratio: 1;
            border: 1px solid rgba(255, 105, 180, 0.15);
        }

        .cell:hover {
            background: rgba(255, 105, 180, 0.15);
            transform: scale(1.03);
        }

        .cell.x {
            color: #ff69b4;
            text-shadow: 0 0 20px rgba(255, 20, 147, 0.6);
        }

        .cell.o {
            color: #87ceeb;
            text-shadow: 0 0 20px rgba(135, 206, 235, 0.6);
        }

        .cell.win {
            background: rgba(255, 215, 0, 0.25) !important;
            animation: winPulse 0.6s ease-in-out infinite alternate;
        }

        @keyframes winPulse {
            from {
                box-shadow: 0 0 15px rgba(255, 215, 0, 0.3);
            }
            to {
                box-shadow: 0 0 35px rgba(255, 215, 0, 0.7);
            }
        }

        .game-status {
            font-size: 1.3rem;
            color: #ffc0cb;
            min-height: 50px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .game-status .reset-btn {
            padding: 8px 25px;
            font-size: 14px;
            background: rgba(255, 105, 180, 0.2);
            border: 1px solid #ff69b4;
            border-radius: 50px;
            color: #ff69b4;
            cursor: pointer;
            transition: 0.3s;
        }

        .game-status .reset-btn:hover {
            background: #ff69b4;
            color: #fff;
        }

        /* ===== PAGE 4: SURPRISE / BALLOONS ===== */
        .surprise-page {
            position: relative;
            z-index: 1;
            text-align: center;
            overflow: hidden;
        }

        .surprise-page h2 {
            font-size: 2.8rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
            margin-bottom: 15px;
        }

        .balloon-container {
            position: relative;
            height: 400px;
            margin: 20px auto;
            max-width: 600px;
        }

        .balloon {
            position: absolute;
            font-size: 60px;
            animation: balloonFly 4s ease-in-out infinite;
            cursor: pointer;
            transition: 0.3s;
            user-select: none;
        }

        .balloon:hover {
            transform: scale(1.2);
        }

        @keyframes balloonFly {
            0%,
            100% {
                transform: translateY(0) rotate(0deg);
            }
            25% {
                transform: translateY(-30px) rotate(5deg);
            }
            75% {
                transform: translateY(-20px) rotate(-5deg);
            }
        }

        .pop-message {
            font-size: 2rem;
            color: #ffd700;
            min-height: 70px;
            margin-top: 10px;
            animation: popIn 0.5s ease;
        }

        @keyframes popIn {
            0% {
                transform: scale(0);
                opacity: 0;
            }
            70% {
                transform: scale(1.2);
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }

        .confetti-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 999;
        }

        .confetti-piece {
            position: absolute;
            width: 10px;
            height: 10px;
            animation: confettiFall linear forwards;
        }

        @keyframes confettiFall {
            0% {
                transform: translateY(-10vh) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(110vh) rotate(720deg);
                opacity: 0;
            }
        }

        /* ===== PAGE 5: LOVE LETTER ===== */
        .letter-page {
            position: relative;
            z-index: 1;
            text-align: center;
        }

        .letter-page h2 {
            font-size: 2.5rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
        }

        .letter-card {
            max-width: 650px;
            margin: 25px auto;
            background: rgba(255, 182, 193, 0.07);
            border: 2px solid rgba(255, 105, 180, 0.2);
            border-radius: 30px;
            padding: 35px 40px;
            backdrop-filter: blur(12px);
            box-shadow: 0 0 50px rgba(255, 20, 147, 0.1);
            text-align: left;
        }

        .letter-card p {
            color: #ffc0cb;
            font-size: 1.1rem;
            line-height: 2;
            margin-bottom: 15px;
            opacity: 0;
            animation: fadeInLine 0.8s ease forwards;
        }

        .letter-card p:nth-child(1) {
            animation-delay: 0.2s;
        }
        .letter-card p:nth-child(2) {
            animation-delay: 0.8s;
        }
        .letter-card p:nth-child(3) {
            animation-delay: 1.4s;
        }
        .letter-card p:nth-child(4) {
            animation-delay: 2s;
        }
        .letter-card p:nth-child(5) {
            animation-delay: 2.6s;
        }
        .letter-card p:nth-child(6) {
            animation-delay: 3.2s;
        }

        @keyframes fadeInLine {
            to {
                opacity: 1;
                transform: translateY(0);
            }
            from {
                opacity: 0;
                transform: translateY(15px);
            }
        }

        .letter-card .signature {
            font-size: 1.5rem;
            color: #ff69b4;
            text-align: right;
            font-style: italic;
            margin-top: 20px;
        }

        /* ===== PAGE 6: PHOTO GALLERY / OUR MEMORIES ===== */
        .memories-page {
            position: relative;
            z-index: 1;
            text-align: center;
        }

        .memories-page h2 {
            font-size: 2.5rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
        }

        .memory-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            max-width: 800px;
            margin: 30px auto;
        }

        .memory-card {
            background: rgba(255, 182, 193, 0.06);
            border: 1px solid rgba(255, 105, 180, 0.15);
            border-radius: 20px;
            padding: 30px 15px;
            transition: 0.4s;
            cursor: pointer;
        }

        .memory-card:hover {
            transform: translateY(-10px) scale(1.03);
            background: rgba(255, 105, 180, 0.12);
            box-shadow: 0 10px 40px rgba(255, 20, 147, 0.2);
        }

        .memory-card .emoji-big {
            font-size: 3.5rem;
            margin-bottom: 10px;
        }

        .memory-card .memory-text {
            color: #ffc0cb;
            font-size: 1rem;
            font-weight: 500;
        }

        /* ===== RESPONSIVE ===== */
        @media (max-width: 600px) {
            .landing h1 {
                font-size: 2.2rem;
            }
            .landing .big-heart {
                font-size: 80px;
            }
            .navbar .nav-links a {
                font-size: 11px;
                padding: 4px 10px;
            }
            .game-board {
                width: 280px;
                height: 280px;
                padding: 8px;
            }
            .cell {
                font-size: 2.2rem;
            }
            .panda-container img {
                max-width: 250px;
            }
            .letter-card {
                padding: 20px;
            }
            .balloon {
                font-size: 40px;
            }
        }

        /* ===== CURSOR TRAIL ===== */
        .cursor-trail {
            position: fixed;
            pointer-events: none;
            z-index: 9999;
            font-size: 18px;
            animation: trailFade 0.8s ease forwards;
        }

        @keyframes trailFade {
            0% {
                transform: scale(1);
                opacity: 1;
            }
            100% {
                transform: scale(1.5) translateY(-30px);
                opacity: 0;
            }
        }

        /* ===== SPECIAL SURPRISE BUTTON ===== */
        .surprise-btn-area {
            margin-top: 30px;
        }

        .big-surprise-btn {
            padding: 20px 60px;
            font-size: 24px;
            background: linear-gradient(135deg, #ff1493, #ff4500, #ff1493);
            background-size: 200% 200%;
            animation: gradientShift 2s ease infinite;
            border: none;
            border-radius: 60px;
            color: #fff;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 0 60px rgba(255, 20, 147, 0.5);
            transition: 0.3s;
        }

        .big-surprise-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 0 80px rgba(255, 20, 147, 0.8);
        }

        @keyframes gradientShift {
            0%,
            100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }

        /* ===== WHISPER / CHOTA PAGE ===== */
        .whisper-page {
            position: relative;
            z-index: 1;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 80vh;
        }

        .whisper-page h2 {
            font-size: 2.8rem;
            color: #ffb6c1;
            text-shadow: 0 0 30px rgba(255, 20, 147, 0.5);
        }

        .whisper-box {
            max-width: 500px;
            margin: 20px auto;
            padding: 30px;
            background: rgba(255, 182, 193, 0.06);
            border-radius: 30px;
            border: 2px solid rgba(255, 105, 180, 0.2);
        }

        .whisper-box p {
            color: #ffc0cb;
            font-size: 1.2rem;
            line-height: 2;
        }

        .whisper-box .big-emoji {
            font-size: 5rem;
            margin: 15px 0;
            animation: heartbeat 1.5s ease-in-out infinite;
        }

        /* message that types itself */
        .typewriter {
            display: inline-block;
            color: #ff99cc;
            font-size: 1.4rem;
            border-right: 3px solid #ff69b4;
            animation: blink 0.8s step-end infinite;
            white-space: nowrap;
            overflow: hidden;
            max-width: 100%;
        }

        @keyframes blink {
            50% {
                border-color: transparent;
            }
        }

        /* star sparkle */
        .sparkle {
            position: fixed;
            pointer-events: none;
            z-index: 9998;
            font-size: 24px;
            animation: sparkleFade 1s ease forwards;
        }

        @keyframes sparkleFade {
            0% {
                transform: scale(0) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: scale(2) rotate(360deg);
                opacity: 0;
            }
        }
    </style>
</head>
<body>

    <!-- ===== FLOATING HEARTS BG ===== -->
    <div class="hearts-bg" id="heartsBg"></div>

    <!-- ===== CONFETTI CONTAINER ===== -->
    <div class="confetti-container" id="confettiContainer"></div>

    <!-- ===== NAVIGATION ===== -->
    <nav class="navbar">
        <div class="logo">💕 Sorry Baby Mera pyara Baacha💕</div>
        <div class="nav-links">
            <a href="#" data-page="landing" class="active">🏠 Home</a>
            <a href="#" data-page="😘"> Kiss</a>
            <a href="#" data-page="game">🎮 Game</a>
            <a href="#" data-page="surprise">🎉 Surprise</a>
            <a href="#" data-page="letter">💌 Letter</a>
            <a href="#" data-page="memories">💖 Memories</a>
            <a href="#" data-page="whisper">🤫 Chota</a>
        </div>
    </nav>

    <!-- ============================================================ -->
    <!-- PAGE 1: LANDING / MAIN APOLOGY                                   -->
    <!-- ============================================================ -->
    <section class="page active" id="page-landing">
        <div class="landing">
            <h1>I'm So Sorry Baby ❤️</h1>
            <p class="subtitle">~ Meri Jaan, Please Gussa Mat Karo ~</p>

            <div class="big-heart" onclick="createHeartBurst(event)">❤️</div>

            <div class="sorry-msg">
                <p>
                    <span class="highlight">My Love, My Wifey, My Everything... 💕</span><br /><br />
                    I know I messed up and I'm really really sorry.<br />
                    You mean the <span class="highlight">WORLD</span> to me and<br />
                    I hate it when you're angry at me. 😔<br /><br />
                    I promise to be better, my jaan.<br />
                    <span class="highlight">You are my life, my happiness, my everything.</span><br /><br />
                    Will you please forgive me? 🥺👉👈
                </p>
            </div>

            <div>
                <button class="btn" onclick="navigateTo('😘')"> See Kiss 💋</button>
                <button class="btn btn-outline" onclick="navigateTo('game')">🎮 Play a Game</button>
            </div>
            <div style="margin-top:15px;">
                <button class="btn btn-outline" onclick="navigateTo('surprise')">🎉 Surprise!</button>
                <button class="btn btn-outline" onclick="navigateTo('letter')">💌 Read Letter</button>
            </div>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 2: PANDA KISS                                            -->
    <!-- ============================================================ -->
    <section class="page" id="page-panda">
        <div class="panda-page">
            <h2> Kiss For You 💋</h2>
            <p style="color:#ff99cc;font-size:1.1rem;">My cute kiss to make you smile... 😘</p>

            <div class="panda-container">
                <!-- ====== CHANGE THIS PATH TO YOUR PANDA GIF ====== -->
                <img src=<img src="https://media.tenor.com/sWWS1gPJcJQAAAAC/panda-kiss.gif"
     alt="Panda Kissing GIF"
     style="max-width:350px;border-radius:30px;box-shadow:0 0 50px rgba(255,105,180,0.3);border:4px solid rgba(255,105,180,0.3);animation:pandaBounce 2s ease-in-out infinite;"
/>
                alt="Panda Kissing GIF"
                onerror="this.src='https://media.tenor.com/sWWS1gPJcJQAAAAC/panda-kiss.gif'; this.onerror='';"
                />

                <div class="panda-kisses">💋😘💋😘💋</div>
                <p class="panda-caption">Mwaah! Mwaah! Mwaah! 🥰</p>
                <p style="color:#ffc0cb;max-width:500px;">
                    This panda is me — giving you a thousand kisses!<br />
                    Every kiss says "I'm sorry my love... please forgive me" 💕
                </p>
                <button class="btn" onclick="navigateTo('game')">🎮 Next: Play Tic Tac Toe ➡️</button>
            </div>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 3: TIC TAC TOE GAME                                      -->
    <!-- ============================================================ -->
    <section class="page" id="page-game">
        <div class="game-page">
            <h2>🎮 Tic Tac Toe — Play with Me!</h2>
            <p class="game-subtitle">If you win... I'll THOUSAND KISSES YOU! 🍝<br />If I win... you have to smile and forgive me! 😊</p>

            <div class="game-container">
                <div class="game-board" id="gameBoard">
                    <div class="cell" data-index="0"></div>
                    <div class="cell" data-index="1"></div>
                    <div class="cell" data-index="2"></div>
                    <div class="cell" data-index="3"></div>
                    <div class="cell" data-index="4"></div>
                    <div class="cell" data-index="5"></div>
                    <div class="cell" data-index="6"></div>
                    <div class="cell" data-index="7"></div>
                    <div class="cell" data-index="8"></div>
                </div>
                <div class="game-status" id="gameStatus">
                    <span>Your turn, baby! ❤️</span>
                    <button class="reset-btn" onclick="resetGame()">🔄 New Game</button>
                </div>
                <button class="btn btn-outline" onclick="navigateTo('surprise')">🎉 See Surprise ➡️</button>
            </div>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 4: SURPRISE / BALLOONS                                   -->
    <!-- ============================================================ -->
    <section class="page" id="page-surprise">
        <div class="surprise-page">
            <h2>🎉 SURPRISE MY LOVE! 🎉</h2>
            <p style="color:#ff99cc;font-size:1.1rem;">Pop the balloons to reveal your surprise messages! 🎈</p>

            <div class="balloon-container" id="balloonContainer">
                <div class="balloon" style="left:5%;animation-delay:0s;" onclick="popBalloon(this)">🎈</div>
                <div class="balloon" style="left:22%;animation-delay:0.5s;" onclick="popBalloon(this)">🎈</div>
                <div class="balloon" style="left:40%;animation-delay:1s;" onclick="popBalloon(this)">🎈</div>
                <div class="balloon" style="left:58%;animation-delay:1.5s;" onclick="popBalloon(this)">🎈</div>
                <div class="balloon" style="left:75%;animation-delay:2s;" onclick="popBalloon(this)">🎈</div>
                <div class="balloon" style="left:90%;animation-delay:2.5s;" onclick="popBalloon(this)">🎈</div>
            </div>

            <div class="pop-message" id="popMessage">✨ Pop a balloon! ✨</div>

            <div class="surprise-btn-area">
                <button class="big-surprise-btn" onclick="bigSurprise()">💥 CLICK FOR BIG SURPRISE 💥</button>
            </div>

            <div style="margin-top:20px;">
                <button class="btn btn-outline" onclick="navigateTo('letter')">💌 Next: Love Letter ➡️</button>
            </div>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 5: LOVE LETTER                                          -->
    <!-- ============================================================ -->
    <section class="page" id="page-letter">
        <div class="letter-page">
            <h2>💌 A Letter From My Heart 💌</h2>

            <div class="letter-card">
                <p>Meri Jaan, ❤️</p>
                <p>I'm sitting here thinking about us... and about how lucky I am to have you in my life. You are the most beautiful, caring, amazing woman I have ever known.</p>
                <p>I know I made you angry, and I truly am sorry from the bottom of my heart. You don't deserve to be upset because of me. You deserve the world, and I want to spend every day trying to give it to you.</p>
                <p>You are my best friend, my soulmate, my partner in crime, my everything. Life without your smile is like a sky without stars — dark and empty.</p>
                <p>Please forgive this idiot husband of yours. I promise to learn, to grow, and to love you even more every single day. ❤️</p>
                <p>I love you more than words can ever say. You are my forever.</p>
                <div class="signature">~ Yours Forever, Your Hubby 💕</div>
            </div>

            <button class="btn btn-outline" onclick="navigateTo('memories')">💖 Our Memories ➡️</button>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 6: MEMORIES                                             -->
    <!-- ============================================================ -->
    <section class="page" id="page-memories">
        <div class="memories-page">
            <h2>💖 Our Beautiful Journey 💖</h2>
            <p style="color:#ff99cc;font-size:1.1rem;">Every moment with you is a treasure... ✨</p>

            <div class="memory-grid">
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">💑</div>
                    <div class="memory-text">The day we met —<br />my life changed forever</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">💍</div>
                    <div class="memory-text">When you said "Yes" —<br />happiest day of my life</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">🎂</div>
                    <div class="memory-text">Birthdays together —<br />always the best moments</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">🌴</div>
                    <div class="memory-text">Our happiness —<br />laughing nonstop</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">🍜</div>
                    <div class="memory-text">Late night gossip  —<br />our favorite dates</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">🤗</div>
                    <div class="memory-text">Your hugs that make<br />everything better</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">😆</div>
                    <div class="memory-text">The way you laugh —<br />music to my ears</div>
                </div>
                <div class="memory-card" onclick="sparkleClick(this)">
                    <div class="emoji-big">∞</div>
                    <div class="memory-text">Forever with you —<br />that's all I want</div>
                </div>
            </div>

            <button class="btn btn-outline" onclick="navigateTo('whisper')">🤫 One last thing... ➡️</button>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- PAGE 7: WHISPER / CHOTA PAGE                                 -->
    <!-- ============================================================ -->
    <section class="page" id="page-whisper">
        <div class="whisper-page">
            <h2>🤫 Chota Sa Message 🤫</h2>

            <div class="whisper-box">
                <div class="big-emoji">🥺</div>
                <p style="font-size:1.5rem;color:#ff69b4;">
                    <span class="typewriter" id="typewriterText"></span>
                </p>
                <div class="big-emoji">😘</div>
                <p style="color:#ffc0cb;margin-top:10px;">
                    You are my <strong style="color:#ff69b4;">happiness</strong>.<br />
                    Please forgive me and let's be happy again. 💕
                </p>
            </div>

            <div style="margin-top:30px;display:flex;flex-direction:column;align-items:center;gap:15px;">
                <button class="btn" onclick="launchAllConfetti()">💖 Click if You Forgive Me 💖</button>
                <p style="color:#ffc0cb;font-size:0.9rem;">(You know you want to... 😉)</p>
                <button class="btn btn-outline" onclick="navigateTo('landing')">🏠 Back to Home</button>
            </div>
        </div>
    </section>

    <!-- ============================================================ -->
    <!-- JAVASCRIPT                                                    -->
    <!-- ============================================================ -->
    <script>
        // ===== NAVIGATION =====
        function navigateTo(pageId) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            // Show target page
            const target = document.getElementById('page-' + pageId);
            if (target) {
                target.classList.add('active');
            }
            // Update nav links
            document.querySelectorAll('.navbar .nav-links a').forEach(a => {
                a.classList.toggle('active', a.dataset.page === pageId);
            });
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        document.querySelectorAll('.navbar .nav-links a').forEach(a => {
            a.addEventListener('click', function(e) {
                e.preventDefault();
                navigateTo(this.dataset.page);
            });
        });

        // ===== FLOATING HEARTS BG =====
        function createFloatingHearts() {
            const container = document.getElementById('heartsBg');
            const hearts = ['❤️', '💕', '💗', '💖', '💘', '💝', '🩷'];
            for (let i = 0; i < 25; i++) {
                const el = document.createElement('div');
                el.className = 'heart-float';
                el.textContent = hearts[Math.floor(Math.random() * hearts.length)];
                el.style.left = Math.random() * 100 + '%';
                el.style.fontSize = (12 + Math.random() * 25) + 'px';
                el.style.animationDuration = (8 + Math.random() * 12) + 's';
                el.style.animationDelay = (Math.random() * 15) + 's';
                container.appendChild(el);
            }
        }
        createFloatingHearts();

        // ===== HEART BURST ON CLICK =====
        function createHeartBurst(e) {
            const heart = ['❤️', '💕', '💗', '💖', '💘', '💝'];
            for (let i = 0; i < 12; i++) {
                const el = document.createElement('div');
                el.textContent = heart[Math.floor(Math.random() * heart.length)];
                el.className = 'cursor-trail';
                el.style.left = (e.clientX || e.pageX || window.innerWidth / 2) + 'px';
                el.style.top = (e.clientY || e.pageY || window.innerHeight / 2) + 'px';
                el.style.fontSize = (14 + Math.random() * 25) + 'px';
                el.style.animationDuration = (0.8 + Math.random() * 0.6) + 's';
                document.body.appendChild(el);
                setTimeout(() => el.remove(), 1800);
            }
        }

        document.addEventListener('click', function(e) {
            // 30% chance heart burst on any click
            if (Math.random() < 0.3) {
                const heart = ['❤️', '💕', '💗', '💖', '✨'];
                const el = document.createElement('div');
                el.textContent = heart[Math.floor(Math.random() * heart.length)];
                el.className = 'cursor-trail';
                el.style.left = e.clientX + 'px';
                el.style.top = e.clientY + 'px';
                el.style.fontSize = (15 + Math.random() * 20) + 'px';
                document.body.appendChild(el);
                setTimeout(() => el.remove(), 1200);
            }
        });

        // ===== TIC TAC TOE =====
        const gameBoard = document.getElementById('gameBoard');
        const gameStatus = document.getElementById('gameStatus');
        let board = ['', '', '', '', '', '', '', '', ''];
        let currentPlayer = '❤️';
        let gameActive = true;
        let moveCount = 0;

        const winPatterns = [
            [0, 1, 2],
            [3, 4, 5],
            [6, 7, 8],
            [0, 3, 6],
            [1, 4, 7],
            [2, 5, 8],
            [0, 4, 8],
            [2, 4, 6]
        ];

        function checkWinner() {
            for (let pattern of winPatterns) {
                const [a, b, c] = pattern;
                if (board[a] && board[a] === board[b] && board[a] === board[c]) {
                    return { winner: board[a], pattern };
                }
            }
            return null;
        }

        function handleCellClick(e) {
            const cell = e.target;
            const index = parseInt(cell.dataset.index);
            if (!gameActive || board[index] !== '') return;

            board[index] = currentPlayer;
            cell.textContent = currentPlayer;
            cell.classList.add(currentPlayer === '❤️' ? 'x' : 'o');
            moveCount++;

            const result = checkWinner();
            if (result) {
                gameActive = false;
                result.pattern.forEach(i => {
                    document.querySelector(`.cell[data-index="${i}"]`).classList.add('win');
                });
                if (currentPlayer === '❤️') {
                    gameStatus.innerHTML =
                        `<span>🥳 YOU WIN BABY! I'll make dinner! 🍝💕</span><button class="reset-btn" onclick="resetGame()">🔄 Play Again</button>`;
                    launchConfetti(30);
                } else {
                    gameStatus.innerHTML =
                        `<span>😊 I win! Now you HAVE to smile and forgive me! 🤗💕</span><button class="reset-btn" onclick="resetGame()">🔄 Play Again</button>`;
                    launchConfetti(20);
                }
                return;
            }

            if (moveCount === 9) {
                gameActive = false;
                gameStatus.innerHTML =
                    `<span>🤝 It's a tie! Let's play again, baby! 💕</span><button class="reset-btn" onclick="resetGame()">🔄 Play Again</button>`;
                return;
            }

            currentPlayer = currentPlayer === '❤️' ? '😊' : '❤️';
            gameStatus.innerHTML = `<span>${currentPlayer === '❤️' ? "Your turn, baby! ❤️" : "My turn! 😊"}</span>`;
        }

        document.querySelectorAll('.cell').forEach(cell => {
            cell.addEventListener('click', handleCellClick);
        });

        function resetGame() {
            board = ['', '', '', '', '', '', '', '', ''];
            currentPlayer = '❤️';
            gameActive = true;
            moveCount = 0;
            document.querySelectorAll('.cell').forEach(cell => {
                cell.textContent = '';
                cell.className = 'cell';
            });
            gameStatus.innerHTML = `<span>Your turn, baby! ❤️</span><button class="reset-btn" onclick="resetGame()">🔄 New Game</button>`;
        }

        // ===== BALLOON SURPRISE =====
        let balloonMessages = [
            '✨ You are the most beautiful girl in the world! ✨',
            '💖 I love you more than pizza! (And that\'s a LOT!) 💖',
            '🌟 You make my life complete! 🌟',
            '🍫 You\'re sweeter than chocolate! 🍫',
            '🎵 You\'re the melody of my heart! 🎵',
            '👑 You\'re my QUEEN forever! 👑'
        ];
        let poppedBalloons = 0;

        function popBalloon(el) {
            if (el.style.opacity === '0') return;
            el.style.opacity = '0';
            el.style.transform = 'scale(1.5)';
            el.style.transition = '0.3s';
            const msg = balloonMessages[poppedBalloons % balloonMessages.length];
            document.getElementById('popMessage').textContent = '💥 POP! ' + msg;
            document.getElementById('popMessage').style.animation = 'none';
            setTimeout(() => {
                document.getElementById('popMessage').style.animation = 'popIn 0.5s ease';
            }, 10);
            poppedBalloons++;
            launchConfetti(15);

            if (poppedBalloons >= 6) {
                setTimeout(() => {
                    document.getElementById('popMessage').textContent = '🎉 You popped ALL balloons! You\'re amazing! I LOVE YOU! 💕🎉';
                    launchConfetti(50);
                }, 600);
            }
        }

        // ===== BIG SURPRISE =====
        function bigSurprise() {
            launchConfetti(100);
            const msgs = [
                '💖 I LOVE YOU SO MUCH! 💖',
                '🌟 YOU ARE MY EVERYTHING! 🌟',
                '🥰 FORGIVE ME PLEASE! 🥰',
                '💕 YOU\'RE THE BEST WIFE AND PYARA BAACHA EVER! 💕',
                '🎉 LET\'S BE HAPPY TOGETHER! 🎉',
                '😘 MUAAAH! A THOUSAND KISSES! 😘'
            ];
            const msg = msgs[Math.floor(Math.random() * msgs.length)];
            document.getElementById('popMessage').textContent = msg;
            document.getElementById('popMessage').style.animation = 'none';
            setTimeout(() => {
                document.getElementById('popMessage').style.animation = 'popIn 0.5s ease';
            }, 10);

            // Also create many hearts
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const heart = ['❤️', '💕', '💗', '💖', '💘', '💝', '✨', '🌟', '🎉'];
                    const el = document.createElement('div');
                    el.textContent = heart[Math.floor(Math.random() * heart.length)];
                    el.className = 'cursor-trail';
                    el.style.left = (Math.random() * window.innerWidth) + 'px';
                    el.style.top = (Math.random() * window.innerHeight) + 'px';
                    el.style.fontSize = (20 + Math.random() * 40) + 'px';
                    el.style.animationDuration = (1 + Math.random() * 1) + 's';
                    document.body.appendChild(el);
                    setTimeout(() => el.remove(), 2500);
                }, i * 100);
            }
        }

        // ===== CONFETTI =====
        function launchConfetti(count) {
            const container = document.getElementById('confettiContainer');
            const colors = ['#ff1493', '#ff69b4', '#ffd700', '#ff4500', '#00ff7f', '#87ceeb', '#ff6347', '#ff00ff', '#ffff00'];
            for (let i = 0; i < count; i++) {
                const piece = document.createElement('div');
                piece.className = 'confetti-piece';
                piece.style.left = Math.random() * 100 + '%';
                piece.style.top = '-10px';
                piece.style.width = (5 + Math.random() * 10) + 'px';
                piece.style.height = (5 + Math.random() * 10) + 'px';
                piece.style.background = colors[Math.floor(Math.random() * colors.length)];
                piece.style.borderRadius = Math.random() > 0.5 ? '50%' : '2px';
                piece.style.animationDuration = (2 + Math.random() * 3) + 's';
                piece.style.animationDelay = (Math.random() * 1.5) + 's';
                container.appendChild(piece);
                setTimeout(() => piece.remove(), 5000);
            }
        }

        function launchAllConfetti() {
            launchConfetti(120);
            // Also show heart explosion
            for (let i = 0; i < 30; i++) {
                setTimeout(() => {
                    const heart = ['❤️', '💕', '💗', '💖', '💘', '💝', '🎉', '🎊', '✨', '🥰'];
                    const el = document.createElement('div');
                    el.textContent = heart[Math.floor(Math.random() * heart.length)];
                    el.className = 'cursor-trail';
                    el.style.left = (Math.random() * window.innerWidth) + 'px';
                    el.style.top = (Math.random() * window.innerHeight) + 'px';
                    el.style.fontSize = (15 + Math.random() * 35) + 'px';
                    el.style.animationDuration = (1 + Math.random() * 1.5) + 's';
                    document.body.appendChild(el);
                    setTimeout(() => el.remove(), 3000);
                }, i * 80);
            }

            // Show a sweet message
            const status = document.querySelector('.whisper-page .whisper-box');
            if (status) {
                const forgiveMsg = document.createElement('div');
                forgiveMsg.style.cssText =
                    'margin-top:20px;font-size:2rem;color:#ffd700;animation:popIn 0.8s ease;text-shadow:0 0 30px rgba(255,215,0,0.5);';
                forgiveMsg.textContent = '💕 YOU FORGAVE ME! I LOVE YOU FOREVER! 💕';
                status.appendChild(forgiveMsg);
            }

            // Redirect to home after a bit
            setTimeout(() => {
                navigateTo('landing');
            }, 3000);
        }

        // ===== SPARKLE ON MEMORY CLICK =====
        function sparkleClick(el) {
            const sparkles = ['✨', '🌟', '💫', '⭐', '❤️', '💕'];
            for (let i = 0; i < 8; i++) {
                const s = document.createElement('div');
                s.className = 'sparkle';
                s.textContent = sparkles[Math.floor(Math.random() * sparkles.length)];
                s.style.left = (el.offsetLeft + Math.random() * el.offsetWidth) + 'px';
                s.style.top = (el.offsetTop + Math.random() * el.offsetHeight) + 'px';
                s.style.animationDuration = (0.6 + Math.random() * 0.8) + 's';
                document.body.appendChild(s);
                setTimeout(() => s.remove(), 1500);
            }
        }

        // ===== TYPEWRITER EFFECT ON WHISPER PAGE =====
        document.addEventListener('DOMContentLoaded', function() {
            const typeEl = document.getElementById('typewriterText');
            if (!typeEl) return;
            const texts = [
                'Meri Jaan...',
                'You are my world...',
                'I\'m sorry baby...',
                'Please forgive me...',
                'I love you forever...',
                'You are my happiness...',
                'My cute little wife...',
                'I promise to be better...',
                'You mean everything to me...',
                'Choti si baat hai...',
                'Par dil bada hai...',
                'I LOVE YOU! ❤️'
            ];
            let textIndex = 0;
            let charIndex = 0;
            let isDeleting = false;

            function typeEffect() {
                const currentText = texts[textIndex];
                if (!isDeleting) {
                    typeEl.textContent = currentText.substring(0, charIndex + 1);
                    charIndex++;
                    if (charIndex === currentText.length) {
                        isDeleting = true;
                        setTimeout(typeEffect, 2000);
                        return;
                    }
                    setTimeout(typeEffect, 80);
                } else {
                    typeEl.textContent = currentText.substring(0, charIndex - 1);
                    charIndex--;
                    if (charIndex === 0) {
                        isDeleting = false;
                        textIndex = (textIndex + 1) % texts.length;
                        setTimeout(typeEffect, 400);
                        return;
                    }
                    setTimeout(typeEffect, 40);
                }
            }

            // Observer to start typing when page is visible
            const observer = new MutationObserver(() => {
                const whisperPage = document.getElementById('page-whisper');
                if (whisperPage && whisperPage.classList.contains('active') && typeEl.textContent === '') {
                    setTimeout(typeEffect, 500);
                    observer.disconnect();
                }
            });
            observer.observe(document.querySelector('.page#page-whisper') || document.body, {
                attributes: true,
                attributeFilter: ['class']
            });
        });

        console.log('%c❤️ I LOVE YOU BABY! ❤️', 'font-size:30px;color:#ff1493;text-shadow:2px 2px 5px pink;');
        console.log('%c💕 Made with love for my beautiful wife 💕', 'font-size:16px;color:#ff69b4;');
    </script>

</body>
</html>
