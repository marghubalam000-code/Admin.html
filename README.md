<Web Edit By Marghubur Rahman>
<html lang="Hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>❤️ दिल का राज़ - अनोखा प्रपोजल अनुभव ❤️</title>
    <!-- Google Fonts & Smooth Font -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            user-select: none;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            min-height: 100vh;
            background: linear-gradient(145deg, #ff9a9e 0%, #fad0c4 35%, #fad0c4 70%, #ffdde1 100%);
            font-family: 'Poppins', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            position: relative;
            overflow-x: hidden;
            cursor: pointer;
        }

        /* Unique Glassmorphic Container */
        .glass-card {
            background: rgba(255, 255, 255, 0.25);
            backdrop-filter: blur(15px);
            border-radius: 68px;
            border: 1px solid rgba(255,255,240,0.5);
            box-shadow: 0 25px 50px -12px rgba(0,0,0,0.3), inset 0 1px 2px rgba(255,255,255,0.6);
            width: 100%;
            max-width: 550px;
            padding: 25px 20px 40px;
            transition: all 0.3s ease;
            text-align: center;
            z-index: 10;
            position: relative;
        }

        h1 {
            font-size: 2rem;
            font-weight: 800;
            background: linear-gradient(135deg, #ff2e63, #ff7b89);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 2px 2px 15px rgba(0,0,0,0.1);
            margin-bottom: 15px;
            letter-spacing: -0.5px;
        }

        .sub {
            font-weight: 500;
            color: #590d22;
            background: rgba(255,245,240,0.7);
            display: inline-block;
            padding: 5px 18px;
            border-radius: 40px;
            font-size: 0.9rem;
            margin-bottom: 20px;
        }

        /* Input Area */
        .input-group {
            margin: 20px 0;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .input-field {
            background: rgba(255,255,245,0.9);
            border: none;
            border-radius: 60px;
            padding: 14px 20px;
            font-size: 1rem;
            font-family: 'Poppins', sans-serif;
            outline: none;
            text-align: center;
            transition: 0.2s;
            box-shadow: 0 5px 10px rgba(0,0,0,0.05);
            font-weight: 500;
        }

        .input-field:focus {
            transform: scale(1.02);
            background: white;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        /* Photo Upload */
        .photo-label {
            background: #ffb7b2;
            padding: 12px;
            border-radius: 50px;
            font-weight: 600;
            color: #4a0e2e;
            cursor: pointer;
            transition: 0.2s;
            display: inline-block;
            width: fit-content;
            margin: 0 auto;
            backdrop-filter: blur(4px);
        }

        .photo-label:hover {
            background: #ff8a7a;
            transform: scale(1.02);
        }

        #photoPreview {
            width: 90px;
            height: 90px;
            object-fit: cover;
            border-radius: 50%;
            border: 3px solid white;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
            margin: 10px auto;
            display: none;
            background: #ffe0e0;
        }

        .btn-magic {
            background: linear-gradient(95deg, #ff416c, #ff4b2b);
            border: none;
            padding: 14px 25px;
            font-size: 1.3rem;
            font-weight: bold;
            color: white;
            border-radius: 50px;
            cursor: pointer;
            width: 80%;
            margin: 20px auto 10px;
            transition: all 0.3s;
            box-shadow: 0 15px 25px -8px rgba(0,0,0,0.3);
            font-family: monospace;
            letter-spacing: 1px;
        }

        .btn-magic:active {
            transform: scale(0.96);
        }

        /* Floating Heart Canvas & Emojis */
        .heart-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 9999;
        }

        .floating-item {
            position: absolute;
            font-size: 2rem;
            animation: floatUp 5s linear forwards;
            filter: drop-shadow(0 0 5px crimson);
            pointer-events: none;
        }

        @keyframes floatUp {
            0% {
                transform: translateY(100vh) scale(0.5) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-20vh) scale(1.5) rotate(20deg);
                opacity: 0;
            }
        }

        /* Heart tap zone */
        .heart-tap-area {
            background: radial-gradient(circle, rgba(255,220,220,0.9) 0%, rgba(255,180,180,0.4) 100%);
            border-radius: 80px;
            padding: 20px 15px;
            margin: 20px 0;
            cursor: pointer;
            transition: 0.2s;
            border: 2px dashed #ff4d6d;
        }

        .big-heart {
            font-size: 5rem;
            transition: transform 0.1s ease;
            display: inline-block;
        }

        .heart-tap-area:active .big-heart {
            transform: scale(0.85);
        }

        .surprise-name {
            font-size: 1.8rem;
            font-weight: 800;
            color: #c9184a;
            margin-top: 10px;
            background: rgba(255,255,210,0.7);
            border-radius: 50px;
            padding: 5px;
        }

        .shayari-box {
            background: rgba(255, 245, 235, 0.85);
            border-radius: 40px;
            padding: 15px;
            margin: 20px 0;
            font-style: italic;
            font-weight: 500;
            color: #4a0e2e;
            border-left: 6px solid #ff477e;
            font-size: 1rem;
            line-height: 1.4;
            transition: all 0.2s;
        }

        .footer-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .mini-btn {
            background: rgba(255,240,230,0.9);
            border: none;
            border-radius: 40px;
            padding: 6px 18px;
            font-weight: 600;
            font-size: 0.8rem;
            cursor: pointer;
            transition: 0.2s;
            color: #b13e5c;
        }

        .photo-frame-animation {
            position: fixed;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            border: 3px solid gold;
            box-shadow: 0 0 15px rgba(255,215,0,0.7);
            background-size: cover;
            background-position: center;
            z-index: 9998;
            pointer-events: none;
            animation: floatPhoto 7s linear infinite;
        }

        @keyframes floatPhoto {
            0% {
                transform: translate(0, 0) rotate(0deg);
                opacity: 0.8;
            }
            25% {
                transform: translate(30px, -40px) rotate(5deg);
            }
            50% {
                transform: translate(-20px, -90px) rotate(-3deg);
                opacity: 1;
            }
            75% {
                transform: translate(40px, -130px) rotate(6deg);
            }
            100% {
                transform: translate(-30px, -200px) rotate(-5deg);
                opacity: 0;
            }
        }

        @media (max-width: 550px) {
            .glass-card {
                padding: 20px 15px;
            }
            .big-heart {
                font-size: 4rem;
            }
        }
    </style>
</head>
<body>

<div class="heart-canvas" id="floatingCanvas"></div>
<div id="photoFrameContainer"></div>

<div class="glass-card">
    <h1>✨ मेरी दिल की बात ✨</h1>
    <div class="sub">❤️ एक ख़ास एहसास ❤️</div>

    <!-- Name Input -->
    <div class="input-group">
        <input type="text" id="personName" class="input-field" placeholder="अपना नाम लिखिए... (जैसे 'आर्या' या 'सिया')" autocomplete="off">
        
        <!-- Photo Upload Option -->
        <label class="photo-label" for="photoUpload">📸 अपनी फोटो अपलोड करें (Heart Frame में उड़ेगी)</label>
        <input type="file" id="photoUpload" accept="image/*" style="display: none;">
        <img id="photoPreview" alt="preview">
    </div>

    <!-- Tap the Heart -->
    <div class="heart-tap-area" id="heartTapZone">
        <div class="big-heart" id="bigHeartEmoji">❤️</div>
        <div class="surprise-name" id="nameDisplay">💖 दिल पर टैप करें 💖</div>
    </div>

    <!-- Romantic Shayari Section (Dynamic) -->
    <div class="shayari-box" id="shayariBox">
        ❝ हर सुबह तेरी याद, हर शाम तेरा नाम,
        तू आए तो बहारें आए, तू ना आए तो सब बेकाम। ❞
    </div>

    <div class="footer-buttons">
        <button class="mini-btn" id="newShayariBtn">✨ नई शायरी ✨</button>
        <button class="mini-btn" id="burstHeartsBtn">💥 दिलों की बौछार 💥</button>
        <button class="mini-btn" id="resetPhotoBtn">🖼️ फोटो रीसेट</button>
    </div>
    <div style="margin-top: 15px; font-size: 0.7rem; opacity: 0.7;">❤️ हर जगह उड़ते दिल... हर दिल पे तुम्हारा नाम ❤️</div>
</div>

<script>
    // ------------------- ROMANTIC SHAYARI COLLECTION (हिंदी + उर्दू style) ------------------
    const shayariList = [
        "❝ तुमसे मिलकर लगा, जैसे सदियों से जानता हूँ, हर दिल की धड़कन अब तुम्हारा नाम लेती है। ❞",
        "❝ तेरी एक मुस्कान, मेरी दुनिया बदल दे, तू रहे साथ तो हर गम पिघल जाए। ❞",
        "❝ इश्क़ का दरिया है बेहद गहरा, तुम गोता लगाओ तो मंज़र नया हो। ❞",
        "❝ चाँद से खूबसूरत हो, सितारों से रौशन, हर दिल की धड़कन में बसती हो तुम। ❞",
        "❝ तुम्हारे बिना ये दिल सूना सूना, तुम हो तो हर पल लगे नशा सा। ❞",
        "❝ हर दिल पर तेरा नाम लिखा है, किस्मत ने हमको तेरे लिए बनाया है। ❞",
        "❝ तू है तो मेरे पास सब कुछ है, वरना दुनिया में क्या रखा है। ❞",
        "❝ तेरे नाम का दीपक जलाए रखूंगा, हर जनम में तुझे ही पाऊंगा। ❞",
        "❝ आँखों में तुम, सपनों में तुम, अब तो रूह में भी तुम्ही बसते हो। ❞",
        "❝ मेरे दिल की हर धड़कन तुझसे ही जुड़ी है, तू आए तो खुशियों की बारिश हो। ❞"
    ];

    let currentName = "";
    let currentPhotoData = null;   // base64
    let activePhotoFrames = [];
    let heartInterval = null;
    let floatingInterval = null;

    // DOM Elements
    const personNameInput = document.getElementById('personName');
    const heartTapZone = document.getElementById('heartTapZone');
    const nameDisplaySpan = document.getElementById('nameDisplay');
    const shayariBox = document.getElementById('shayariBox');
    const newShayariBtn = document.getElementById('newShayariBtn');
    const burstHeartsBtn = document.getElementById('burstHeartsBtn');
    const resetPhotoBtn = document.getElementById('resetPhotoBtn');
    const photoUpload = document.getElementById('photoUpload');
    const photoPreview = document.getElementById('photoPreview');

    // Helper: create floating heart emoji or custom heart + Name Tag
    function createFloatingHeart(isSpecial = false, customText = null) {
        const canvas = document.getElementById('floatingCanvas');
        const floatingDiv = document.createElement('div');
        floatingDiv.classList.add('floating-item');
        
        let content = '';
        if (customText) {
            content = customText;
        } else {
            // random heart emoji style
            const hearts = ['❤️', '💖', '💗', '💓', '💕', '💘', '💝'];
            const randomHeart = hearts[Math.floor(Math.random() * hearts.length)];
            if (currentName && currentName.trim() !== "" && Math.random() > 0.5) {
                content = `${randomHeart} ${currentName} ${randomHeart}`;
            } else {
                content = randomHeart;
            }
        }
        floatingDiv.innerHTML = content;
        floatingDiv.style.fontSize = (Math.random() * 20 + 20) + 'px'; // 20px to 40px
        floatingDiv.style.left = Math.random() * 100 + '%';
        floatingDiv.style.animationDuration = (Math.random() * 4 + 4) + 's'; // 4-8 sec
        floatingDiv.style.whiteSpace = 'nowrap';
        canvas.appendChild(floatingDiv);
        setTimeout(() => { if(floatingDiv && floatingDiv.remove) floatingDiv.remove(); }, 5000);
    }

    // Burst of many hearts (surprise)
    function burstHearts(count = 35) {
        for (let i = 0; i < count; i++) {
            setTimeout(() => {
                createFloatingHeart(true);
            }, i * 40);
        }
        // also add name hearts if name exists
        if (currentName && currentName.trim() !== "") {
            for (let i = 0; i < 15; i++) {
                setTimeout(() => {
                    createFloatingHeart(false, `💗 ${currentName} 💗`);
                }, i * 80);
            }
        }
    }

    // create continuous floating hearts ( romantic environment )
    function startContinuousHearts() {
        if (heartInterval) clearInterval(heartInterval);
        heartInterval = setInterval(() => {
            if (document.hasFocus()) {
                createFloatingHeart();
            }
        }, 800);
    }

    // Stop continuous hearts (optional)
    function stopContinuousHearts() {
        if (heartInterval) clearInterval(heartInterval);
        heartInterval = null;
    }

    // SPECIAL: photo floating frames (if photo uploaded)
    function startPhotoFloating() {
        // remove old frames
        const container = document.getElementById('photoFrameContainer');
        while (container.firstChild) container.removeChild(container.firstChild);
        activePhotoFrames = [];
        if (!currentPhotoData) return;

        // create multiple floating photo frames (Heart shaped circular frames)
        const numFrames = 6; 
        for (let i = 0; i < numFrames; i++) {
            const frame = document.createElement('div');
            frame.classList.add('photo-frame-animation');
            frame.style.backgroundImage = `url('${currentPhotoData}')`;
            frame.style.width = '70px';
            frame.style.height = '70px';
            frame.style.borderRadius = '50%';
            frame.style.border = '3px solid #ff66b2';
            frame.style.boxShadow = '0 0 20px #ff3366';
            frame.style.left = Math.random() * 80 + 10 + '%';
            frame.style.animationDuration = (Math.random() * 5 + 6) + 's';
            frame.style.animationDelay = (i * 0.8) + 's';
            container.appendChild(frame);
            activePhotoFrames.push(frame);
            // remove after animation ends
            frame.addEventListener('animationend', () => {
                if(frame && frame.remove) frame.remove();
            });
        }
        // re-generate floating frames every 9 sec to keep them flowing
        if (floatingInterval) clearInterval(floatingInterval);
        floatingInterval = setInterval(() => {
            if (currentPhotoData && document.body.contains(container)) {
                const newFrame = document.createElement('div');
                newFrame.classList.add('photo-frame-animation');
                newFrame.style.backgroundImage = `url('${currentPhotoData}')`;
                newFrame.style.width = '70px';
                newFrame.style.height = '70px';
                newFrame.style.borderRadius = '50%';
                newFrame.style.border = '3px solid gold';
                newFrame.style.left = Math.random() * 85 + 5 + '%';
                newFrame.style.animationDuration = (Math.random() * 5 + 5) + 's';
                container.appendChild(newFrame);
                newFrame.addEventListener('animationend', () => newFrame.remove());
            }
        }, 4000);
    }

    function stopPhotoFloating() {
        if (floatingInterval) clearInterval(floatingInterval);
        floatingInterval = null;
        const container = document.getElementById('photoFrameContainer');
        while (container.firstChild) container.removeChild(container.firstChild);
    }

    // update photo preview and reset floating
    function updatePhoto(file) {
        if (!file) return;
        const reader = new FileReader();
        reader.onload = function(e) {
            currentPhotoData = e.target.result;
            photoPreview.src = currentPhotoData;
            photoPreview.style.display = 'block';
            // restart photo floating
            stopPhotoFloating();
            startPhotoFloating();
            // also show a toast like surprise
            createFloatingHeart(false, "✨ फोटो Heart फ्रेम में ✨");
            burstHearts(12);
        };
        reader.readAsDataURL(file);
    }

    // MAIN SURPRISE: When user taps on big heart, show their name in romantic way, floating name+hearts
    function handleHeartTap() {
        let userName = personNameInput.value.trim();
        if (userName === "") {
            // surprise default if empty
            nameDisplaySpan.innerHTML = "✨ कोई नाम नहीं? ✨<br>❤️ तुम तो अनमोल हो! ❤️";
            createFloatingHeart(false, "💖 अनमोल दिल 💖");
            burstHearts(20);
            shayariBox.innerHTML = "❝ बिना नाम के भी तुम खास हो, दिल की धड़कन हो तुम प्यास हो। ❞";
            return;
        }
        currentName = userName;
        // show name with romantic effect
        nameDisplaySpan.innerHTML = `✨ ${currentName} ✨<br>💖 तुम हो मेरे दिल में 💖`;
        // burst hearts with name
        for(let i=0; i<28; i++) {
            setTimeout(() => {
                createFloatingHeart(false, `❤️ ${currentName} ❤️`);
            }, i*50);
        }
        // update shayari with name touch
        const specialShayari = `❝ ${currentName}, तेरे नाम की मिठास, हर दिल में बसती है प्यास। तू आए तो बहारें, हर सूरत मुस्कुराए। ❞`;
        shayariBox.innerHTML = specialShayari;
        // also extra surprise: create a big floating heart with name animation
        const canvasDiv = document.getElementById('floatingCanvas');
        const bigSpecial = document.createElement('div');
        bigSpecial.classList.add('floating-item');
        bigSpecial.innerHTML = `💘💖💗 ${currentName} 💗💖💘`;
        bigSpecial.style.fontSize = '42px';
        bigSpecial.style.fontWeight = 'bold';
        bigSpecial.style.left = '30%';
        bigSpecial.style.animationDuration = '6s';
        canvasDiv.appendChild(bigSpecial);
        setTimeout(() => bigSpecial.remove(), 5500);
        // if photo available, do extra happy dance frames
        if(currentPhotoData){
            stopPhotoFloating();
            startPhotoFloating();
            // burst special hearts around photos
            for(let f=0;f<10;f++) setTimeout(()=>createFloatingHeart(false, "💕📸💕"), f*100);
        }
    }

    // Random new shayari from list with name insertion possible
    function getRandomShayari() {
        let randomIndex = Math.floor(Math.random() * shayariList.length);
        let selected = shayariList[randomIndex];
        if (currentName && currentName.trim() !== "") {
            // replace some placeholder or just add name in front
            if (Math.random() > 0.5) {
                selected = `✨ ${currentName} ✨ ` + selected;
            } else {
                selected = selected + `  —  ❤️ ${currentName} ❤️`;
            }
        }
        return selected;
    }

    function updateShayariRandom() {
        shayariBox.innerHTML = getRandomShayari();
        // also add little heart effect on change
        createFloatingHeart(false, "✨ नई शायरी ✨");
    }

    // reset photo & remove frames
    function resetPhoto() {
        currentPhotoData = null;
        photoPreview.style.display = 'none';
        photoPreview.src = "";
        photoUpload.value = "";
        stopPhotoFloating();
        // optional message
        createFloatingHeart(false, "🖼️ फोटो हटा दी गई 🖼️");
        shayariBox.innerHTML = "❝ फोटो डालोगे तो दिल के फ्रेम में उड़ोगे ❞";
        setTimeout(() => {
            if(!currentPhotoData) shayariBox.innerHTML = getRandomShayari();
        }, 2000);
    }

    // Event listeners
    heartTapZone.addEventListener('click', (e) => {
        e.stopPropagation();
        handleHeartTap();
    });

    newShayariBtn.addEventListener('click', () => {
        updateShayariRandom();
    });

    burstHeartsBtn.addEventListener('click', () => {
        burstHearts(50);
        if (currentName) {
            for (let i=0; i<20; i++) setTimeout(()=> createFloatingHeart(false, `💖 ${currentName} 💖`), i*60);
        } else {
            createFloatingHeart(false, "💥 प्यार भरा धमाका 💥");
        }
    });

    resetPhotoBtn.addEventListener('click', resetPhoto);

    photoUpload.addEventListener('change', (e) => {
        if (e.target.files && e.target.files[0]) {
            updatePhoto(e.target.files[0]);
        }
    });

    // on window load, start continuous hearts and some initial animation
    window.addEventListener('load', () => {
        startContinuousHearts();
        // default poetic floating
        setInterval(() => {
            if (Math.random() > 0.7 && currentName) {
                createFloatingHeart(false, `💌 ${currentName} 💌`);
            } else if (Math.random() > 0.8){
                createFloatingHeart();
            }
        }, 3000);
        // extra style: if user types name, live preview effect not mandatory but cute
        personNameInput.addEventListener('input', (e) => {
            let typing = e.target.value.trim();
            if(typing !== ""){
                nameDisplaySpan.innerHTML = `💭 ${typing} ... दिल पर टैप करें 💭`;
            } else {
                nameDisplaySpan.innerHTML = "💖 दिल पर टैप करें 💖";
            }
        });
    });

    // cleanup intervals if page gets hidden (optional)
    window.addEventListener('beforeunload', () => {
        if(heartInterval) clearInterval(heartInterval);
        if(floatingInterval) clearInterval(floatingInterval);
    });
</script>
</body>
</html>
