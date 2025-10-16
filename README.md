<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Littavya's 30th Birthday Invitation - Black Owl Surabaya</title>
    <link rel="preload" href="https://fonts.gstatic.com/s/greatvibes/v14/RWmMoKWRJgYcSQc3BVgGzC8c.woff2" as="font" type="font/woff2" crossorigin>
    <link rel="preload" href="https://fonts.gstatic.com/s/poppins/v20/pxiByp8kv8JHgM5WFRfL.woff2" as="font" type="font/woff2" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        /* ========================================================== */
        /* CSS STYLES (IMPROVED UNITS AND ACCESSIBILITY) */
        /* ========================================================== */

        /* Menggunakan rem untuk skala yang lebih baik dan memastikan tampilan potrait yang fokus */
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
            overflow-x: hidden;
            /* Latar belakang bias gold */
            background: radial-gradient(circle at center, rgba(255, 215, 0, 0.1) 0%, rgba(0, 0, 0, 1) 70%);
            background-attachment: fixed;
            /* Memastikan body tidak bergeser */
            min-height: 100vh;
        }
        
        /* ---------------------------------------------------------- */
        /* Landing Page */
        /* ---------------------------------------------------------- */
        #landing-page {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: var(--color-black); z-index: 99; display: flex; flex-direction: column; justify-content: center; align-items: center; transition: opacity 1s ease-in-out; text-align: center;
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
        /* Main Content - Perubahan Utama untuk Potrait */
        /* ---------------------------------------------------------- */
        .container {
            position: relative; 
            z-index: 10; 
            display: none;
            flex-direction: column; 
            align-items: center; 
            /* Ubah min-height menjadi min-height: 100vh; untuk memastikan isi memenuhi layar vertikal */
            min-height: 100vh; 
            text-align: center; 
            padding: 1.25rem; 
            /* Menggunakan padding-bottom yang lebih besar untuk konten yang panjang saat scroll */
            padding-bottom: 5rem;
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
            /* Tambahkan margin-top untuk estetika di layar besar, dan pastikan tidak terlalu besar di ponsel */
            margin-top: 5vh; 
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
            /* Ukuran font disesuaikan untuk nama yang lebih panjang */
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
            .title-name { font-size: 3.5rem; } /* Disesuaikan untuk nama yang lebih panjang */
            .title-age { font-size: 4rem; }
            .time-value { font-size: 1.8rem; }
            #countdown { gap: 0.5rem; }
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

                <p class="detail-item">
                    **Time:** 7.00 PM WIB - Finish
                </p>
                
                <div class="detail-item">
                    <span class="venue-name">
                        Black Owl Surabaya
                    </span>
                    <span class="venue-location">
                        Room Jackson
                        <br>
                        [Lokasi Pesta]
                    </span>
                </div>

                <p class="dresscode">Dresscode: <span>BLACK GOLD</span></p>
            </section>
            
            <section class="countdown-section">
                <h3 style="color:var(--color-gold); font-size:1.1em; margin-bottom:10px;">Countdown to the Event</h3>
                
                <div id="countdown" aria-live="polite">
                    <div><span class="time-value" id="days">00</span><span class="time-label">Days</span></div>
                    <div><span class="time-value" id="hours">00</span><span class="time-label">Hours</span></div>
                    <div><span class="time-value" id="minutes">00</span><span class="time-label">Minutes</span></div>
                    <div><span class="time-value" id="seconds">00</span><span class="time-label">Seconds</span></div>
                </div>
            </section>

            <section class="location-section">
                <h3 style="color:var(--color-gold); font-size:1.1em;">Location Map</h3>
                
                <div class="map-container">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3957.510345091807!2d112.7238242!3d-7.2929427!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2dd7fbdf936e4f3f%3A0x6e26922384a622a7!2sBlack%20Owl%20Dine%20%26%20Wines%20Surabaya!5e0!3m2!1sen!2sid!4v1717315200000!5m2!1sen!2sid"
                        title="Map to Black Owl Surabaya"
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
                
                <a href="https://maps.app.goo.gl/95tY7Q3nQYg5d625A" target="_blank" class="cta-button">
                    Get Directions (Google Maps)
                </a>
            </section>
            
            <section class="rsvp-section">
                <h3 style="color:var(--color-gold); font-size:1.1em;">RSVP</h3>
                <p style="font-size:0.9em; opacity:0.9;">Kindly confirm your attendance:</p>
                <button class="cta-button rsvp-button" onclick="handleRsvp('attend');">I Will Attend</button>
                <button class="cta-button rsvp-button" style="background: white; color: black; margin-left: 10px;" onclick="handleRsvp('decline');">Regretfully Decline</button>
            </section>
            
        </article>
        
        <p style="margin-top: 40px; font-size: 0.8em; color: #aaa; opacity:0.7;">See you at Black Owl!</p>

    </main>

    <button id="music-button" onclick="toggleMusic()" style="display: none;" aria-label="Play/Pause Background Music">♫</button> 

    <script>
        // ==========================================================
        // JAVASCRIPT LOGIC 
        // ==========================================================

        const music = document.getElementById('party-music');
        const musicButton = document.getElementById('music-button');
        const landingPage = document.getElementById('landing-page');
        const mainInvitation = document.getElementById('main-invitation');
        let musicPlaying = false; 

        // Function to open the invitation (triggered by "Invitation" button)
        function openInvitation() {
            // Attempt to play music, only update state/button on success
            music.play().then(() => {
                musicPlaying = true;
                musicButton.innerHTML = '♫'; 
            }).catch(error => {
                console.warn("Autoplay was blocked:", error);
                musicButton.innerHTML = '♪'; 
            });

            // Hide landing page with fade out transition
            landingPage.style.opacity = '0';
            setTimeout(() => {
                landingPage.style.display = 'none';
                mainInvitation.style.display = 'flex'; // Show main content
                musicButton.style.display = 'block'; // Show music button
            }, 1000); 
        }

        // Function to control music (Play/Pause)
        function toggleMusic() {
            if (musicPlaying) {
                music.pause();
                musicButton.innerHTML = '♪'; 
                musicPlaying = false;
            } else {
                music.play().then(() => {
                    musicButton.innerHTML = '♫'; 
                    musicPlaying = true;
                }).catch(error => {
                    console.error("Playback failed:", error);
                });
            }
        }

        // RSVP function
        function handleRsvp(status) {
            // ENGLISH ALERT MESSAGES
            if (status === 'attend') {
                alert('Thank you! Your RSVP has been received.');
            } else {
                alert('We will miss you! If you change your mind, let Littavya know.');
            }
        }
        
        // ----------------------------------------------------------
        // Countdown Timer & Background Animation
        // ----------------------------------------------------------
        const targetDate = new Date("Oct 28, 2025 19:00:00").getTime(); 
        const countdownFunction = setInterval(function() {
            const now = new Date().getTime();
            const distance = targetDate - now;
            
            let days = Math.floor(distance / (1000 * 60 * 60 * 24));
            let hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            let minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            let seconds = Math.floor((distance % (1000 * 60)) / 1000);
            
            const formatTime = (time) => time < 10 ? '0' + time : time;

            document.getElementById("days").innerHTML = formatTime(days);
            document.getElementById("hours").innerHTML = formatTime(hours);
            document.getElementById("minutes").innerHTML = formatTime(minutes);
            document.getElementById("seconds").innerHTML = formatTime(seconds);

            if (distance < 0) {
                clearInterval(countdownFunction);
                document.getElementById("countdown").innerHTML = "<h3 style='color:var(--color-gold);'>THE PARTY IS LIVE!</h3>";
            }
        }, 1000);
        
        // Background Animation
        const particleContainer = document.getElementById('particle-bg');
        const numParticles = 80;
        const particleColors = [
            'var(--color-gold)', 'var(--color-light-gold)', 'var(--color-cream)', 'rgba(255, 255, 255, 0.7)'
        ];

        for (let i = 0; i < numParticles; i++) {
            const particle = document.createElement('div');
            particle.classList.add('particle');
            const size = Math.random() * 4 + 1;
            const left = Math.random() * 100;
            const duration = Math.random() * 20 + 10;
            const delay = Math.random() * 20;
            const color = particleColors[Math.floor(Math.random() * particleColors.length)];
            particle.style.width = `${size}px`;
            particle.style.height = `${size}px`;
            particle.style.left = `${left}vw`;
            particle.style.animationDuration = `${duration}s`;
            particle.style.animationDelay = `${delay}s`;
            particle.style.backgroundColor = color;
            particle.style.opacity = Math.random() * 0.6 + 0.3;
            particleContainer.appendChild(particle);
        }
    </script>
</body>
</html>
