
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Littavya 30th Birthday Invitation - Black Owl Surabaya</title>
    <link rel="preload" href="https://fonts.gstatic.com/s/greatvibes/v14/RWmMoKWRJgYcSQc3BVgGzC8c.woff2" as="font" type="font/woff2" crossorigin>
    <link rel="preload" href="https://fonts.gstatic.com/s/poppins/v20/pxiByp8kv8JHgM5WFRfL.woff2" as="font" type="font/woff2" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        /* ========================================================== */
        /* CSS STYLES (IMPROVED UNITS AND STABILITY) */
        /* ========================================================== */

        /* Mengatur HTML dan BODY untuk stabilitas tinggi layar */
        html, body {
            height: 100%;
            /* Mengizinkan scroll vertikal secara umum jika konten melebihi layar */
            overflow-x: hidden; /* Tetap sembunyikan scroll horizontal yang tidak perlu */
        }
        
        :root {
            --color-black: #000000;
            --color-gold: #FFD700;
            --color-light-gold: #FFEA9F;
            --color-cream: #FFFDD0;
            --color-red: #FF0000;
            --font-script: 'Great Vibes', cursive;
            --font-main: 'Poppins', sans-serif;
            font-size: 16px; /* Base font size */
        }

        body {
            margin: 0; padding: 0; 
            color: white; 
            font-family: var(--font-main); 
            /* overflow-x: hidden; Dihapus karena sudah ada di html, body */
            
            /* Latar belakang bias gold */
            background: radial-gradient(circle at center, rgba(255, 215, 0, 0.1) 0%, rgba(0, 0, 0, 1) 70%);
            background-attachment: fixed; /* Latar belakang tetap saat scroll */
        }
        
        /* ---------------------------------------------------------- */
        /* Landing Page */
        /* ---------------------------------------------------------- */
        #landing-page {
            position: fixed; top: 0; left: 0; width: 100%; height: 100vh; /* Menggunakan 100vh untuk memastikan penuh layar */
            background-color: var(--color-black); z-index: 99; display: flex; flex-direction: column; justify-content: center; align-items: center; transition: opacity 1s ease-in-out; text-align: center;
        }
        #landing-page .intro-text {
            color: white; 
            font-size: 1.25rem; 
            margin-bottom: 1.25rem; 
            font-weight: 300;
        }
        #landing-page .intro-name {
            font-family: var(--font-script); 
            font-size: 3.5rem; 
            color: var(--color-gold); 
            margin-bottom: 3.125rem;
        }

        /* Main Invitation Button */
        .main-cta-button {
            background: var(--color-gold); 
            color: var(--color-black); 
            border: none; 
            padding: 0.9375rem 2.5rem; 
            font-size: 1.125rem; 
            font-weight: 700; 
            border-radius: 5px; 
            cursor: pointer; 
            text-decoration: none; 
            transition: background 0.3s, transform 0.2s;
            text-transform: uppercase;
        }
        .main-cta-button:hover {
            background: var(--color-light-gold); 
            transform: translateY(-2px);
        }

        /* ---------------------------------------------------------- */
        /* Background Animation */
        /* ---------------------------------------------------------- */
        .particle-bg {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; overflow: hidden; z-index: 1; 
        }
        .particle { position: absolute; border-radius: 50%; opacity: 0.8; animation: moveParticles linear infinite; filter: blur(0.5px); }
        @keyframes moveParticles { 0% { transform: translateY(100vh) scale(0); opacity: 0; } 20% { opacity: 0.6; } 50% { opacity: 0.9; } 80% { opacity: 0.6; } 100% { transform: translateY(-10vh) scale(1); opacity: 0; } }

        /* ---------------------------------------------------------- */
        /* Main Content - Diperbarui untuk fokus portrait */
        /* ---------------------------------------------------------- */
        .container {
            position: relative; 
            z-index: 10; 
            display: none;
            flex-direction: column; 
            align-items: center; 
            /* Menggunakan min-height: 100vh agar halaman undangan minimal 1 layar penuh */
            min-height: 100vh; 
            text-align: center; 
            padding: 1.25rem; 
            padding-bottom: 5rem;
            /* Flexbox mengatur posisi di tengah jika konten tidak memenuhi 100vh */
            justify-content: center; 
        }
        /* Media query untuk layar besar agar konten tidak terlalu menempel ke atas/bawah */
        @media (min-height: 800px) {
            .container {
                justify-content: center; /* Memastikan frame di tengah layar besar */
            }
        }

        /* Invitation Frame and Text Styling */
        .invitation-frame { 
            background: rgba(0, 0, 0, 0.85); 
            border: 4px solid var(--color-gold); 
            padding: 2.5rem 1.875rem; 
            max-width: 31.25rem; 
            width: 90%; 
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.6); 
            border-radius: 5px; 
            position: relative; 
            margin-top: 5vh; /* Sedikit jarak atas */
            margin-bottom: 5vh; /* Sedikit jarak bawah untuk elemen lain */
        }
        /* ... frame decorations (dibiarkan dalam px) ... */
        .invitation-frame::before, .invitation-frame::after { content: ''; position: absolute; background: var(--color-gold); width: 30px; height: 4px; }
        .invitation-frame::before { top: -4px; left: -4px; }
        .invitation-frame::after { top: -4px; right: -4px; }
        .invitation-frame .corner-deco { position: absolute; width: 50px; height: 50px; border: 2px solid var(--color-gold); border-radius: 20px; }
        .invitation-frame .corner-deco.top-left { top: -20px; left: -20px; border-bottom: none; border-right: none; transform: rotate(45deg); }
        .invitation-frame .corner-deco.top-right { top: -20px; right: -20px; border-bottom: none; border-left: none; transform: rotate(-45deg); }
        
        .header-content { margin-bottom: 1.875rem; }
        .title-sub { 
            font-size: 1rem; 
            letter-spacing: 2px; 
            color: white; 
            margin-bottom: 0.3125rem; 
            font-weight: 300;
        }
        .title-name { 
            font-family: var(--font-script); 
            font-size: 4rem; 
            line-height: 1; 
            color: var(--color-gold); 
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7); 
            margin: 0; 
        }
        .title-age { 
            font-family: var(--font-script); 
            font-size: 5rem; 
            color: white; 
            line-height: 0.8; 
            margin-top: -1.875rem; 
            font-weight: 400; 
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.5); 
        }
        
        .details-section { margin-top: 1.25rem; }
        .invitation-intro-text {
            margin-top:0; 
            font-size: 1.125rem; 
            color: rgba(255,255,255,0.9);
            font-weight: 500;
        }

        .detail-item { 
            margin: 0.625rem 0; 
            font-size: 1rem; 
            color: white; 
            line-height: 1.4; 
        }
        .detail-item span.venue-name {
             font-weight: 700;
             color: var(--color-gold);
             display: block;
        }
        .detail-item span.venue-location {
            font-size:0.8em; 
            opacity:0.8;
            display: block;
            font-weight: 300;
        }
        .dresscode { 
            font-size: 1.125rem; 
            font-weight: 700; 
            color: white; 
            margin-top: 1.5625rem; 
        }
        .dresscode span { color: var(--color-gold); }
        
        /* ---------------------------------------------------------- */
        /* Countdown Timer CSS */
        /* ---------------------------------------------------------- */
        #countdown { 
            margin: 1.875rem 0 1.25rem; 
            padding: 0.9375rem 0; 
            display: flex; 
            justify-content: center;
            gap: 0.9375rem; 
            flex-wrap: wrap; 
        }
        #countdown > div { 
            display: flex; 
            flex-direction: column; 
            align-items: center;
            text-align: center;
        }
        .time-value { 
            display: block; 
            font-size: 2rem; 
            font-weight: 700; 
            color: var(--color-red); 
            text-shadow: 0 0 8px rgba(255, 0, 0, 0.5); 
            line-height: 1.1;
        }
        .time-label { 
            font-size: 0.8125rem; 
            color: white; 
            text-transform: uppercase;
        }

        /* ---------------------------------------------------------- */
        /* Location & Buttons */
        /* ---------------------------------------------------------- */
        .location-section { width: 100%; margin-top: 1.875rem; }
        .map-container { border: 2px solid var(--color-gold); height: 15.625rem; margin-top: 0.9375rem; overflow: hidden; box-shadow: 0 0 10px rgba(255, 215, 0, 0.4); }
        .map-container iframe { width: 100%; height: 100%; border: none; }
        .cta-button { 
            background: var(--color-gold); 
            color: var(--color-black); 
            border: none; 
            padding: 0.625rem 1.25rem; 
            font-size: 1rem; 
            font-weight: 700; 
            border-radius: 5px; 
            cursor: pointer; 
            margin-top: 1.25rem; 
            text-decoration: none; 
            display: inline-block; 
            transition: background 0.3s, transform 0.2s; 
            text-transform: uppercase; 
        }
        .cta-button:hover { background: var(--color-light-gold); transform: translateY(-2px); }
        .rsvp-section { margin-top: 2.5rem; padding-top: 1.25rem; border-top: 1px dashed rgba(255, 215, 0, 0.3); }
        .rsvp-section button { margin: 0.3125rem; }
        
        #music-button { 
            position: fixed; 
            bottom: 1.25rem; 
            right: 1.25rem; 
            z-index: 100; 
            background: rgba(255, 215, 0, 0.9); 
            border: none; 
            border-radius: 50%; 
            width: 3.125rem; 
            height: 3.125rem; 
            line-height: 3.125rem; 
            text-align: center; 
            font-size: 1.25rem; 
            cursor: pointer; 
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3); 
            color: var(--color-black); 
        }

        @media (max-width: 600px) { 
            .title-name { font-size: 3.5rem; }
            .title-age { font-size: 4rem; }
            .time-value { font-size: 1.8rem; }
            #countdown { gap: 0.5rem; }
            /* Penyesuaian frame di mobile agar tidak terlalu memakan margin vertikal */
            .invitation-frame {
                margin-top: 2rem;
                margin-bottom: 2rem;
            }
        }
    </style>
</head>
<body>
    
    <audio id="party-music" loop aria-label="Background party music">
        <source src="http://googleusercontent.com/file_content/0" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <header id="landing-page" role="banner">
        <p class="intro-text">You are invited to the birthday celebration of</p>
        <h1 class="intro-name">Littavya</h1>
        <button class="main-cta-button" onclick="openInvitation()">Open Invitation</button>
    </header>

    <div class="particle-bg" id="particle-bg" aria-hidden="true"></div>

    <main class="container" id="main-invitation" role="main">
        <article class="invitation-frame">
            
            <div class="corner-deco top-left" aria-hidden="true"></div>
            <div class="corner-deco top-right" aria-hidden="true"></div>
            
            <header class="header-content">
                <p class="title-sub">Birthday Invitation</p>
                <hgroup>
                    <h1 class="title-name">Littavya</h1>
                    <h2 class="title-age">30</h2>
                </hgroup>
            </header>

            <section class="details-section">
                <p class="invitation-intro-text">
                    We are thrilled to invite you to celebrate this special day.
                </p>
                
                <p class="detail-item">
                    **Date:** Saturday, October 28, 2025
                </p>
