<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday! ✨</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #e0f2fe 0%, #bae6fd 35%, #f0f9ff 70%, #ffffff 100%);
      background-size: 300% 300%;
      animation: blueShift 12s ease infinite;
      padding: 20px;
      overflow-x: hidden;
      overflow-y: auto;
      position: relative;
      color: #1e293b;
    }

    /* Pattern Kaligrafi Love di Background */
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-image: radial-gradient(rgba(56, 189, 248, 0.15) 1px, transparent 0),
                        url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='160' height='160' viewBox='0 0 160 160'%3E%3Cg fill='none' stroke='%230284c7' stroke-width='1.5' opacity='0.09'%3E%3Cpath d='M80,45 C65,20 30,25 30,55 C30,85 80,120 80,120 C80,120 130,85 130,55 C130,25 95,20 80,45 Z' /%3E%3Cpath d='M80,55 C70,38 45,40 45,60 C45,80 80,105 80,105 C115,80 90,38 80,55 Z' stroke-dasharray='2,2' /%3E%3C/g%3E%3C/svg%3E");
      background-size: 80px 80px, 160px 160px;
      pointer-events: none;
      z-index: 0;
    }

    @keyframes blueShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .light-glow {
      position: fixed;
      border-radius: 50%;
      filter: blur(80px);
      opacity: 0.6;
      pointer-events: none;
      z-index: 0;
    }

    .glow-1 {
      width: 340px;
      height: 340px;
      background: radial-gradient(circle, #7dd3fc 0%, rgba(125, 211, 252, 0) 70%);
      top: -5%;
      left: -5%;
    }

    .glow-2 {
      width: 360px;
      height: 360px;
      background: radial-gradient(circle, #e0f2fe 0%, rgba(224, 242, 254, 0) 70%);
      bottom: -5%;
      right: -5%;
    }

    .bg-sparkle-container {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 1;
      overflow: hidden;
    }

    .floating-bg-sparkle {
      position: absolute;
      bottom: -20px;
      border-radius: 50%;
      background: radial-gradient(circle, #ffffff 0%, #38bdf8 60%, rgba(56, 189, 248, 0) 100%);
      box-shadow: 0 0 10px #ffffff, 0 0 20px #38bdf8;
      pointer-events: none;
      opacity: 0;
      animation: floatBgSparkle var(--duration) ease-in-out infinite;
      animation-delay: var(--delay);
    }

    @keyframes floatBgSparkle {
      0% { opacity: 0; transform: translateY(0) scale(0.5); }
      30% { opacity: 0.8; }
      70% { opacity: 0.8; }
      100% { opacity: 0; transform: translateY(-105vh) scale(1.5); }
    }

    .wrapper {
      width: 100%;
      max-width: 440px;
      z-index: 2;
      margin: 20px 0;
    }

    .card {
      display: none;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border-radius: 24px;
      padding: 24px;
      text-align: center;
      box-shadow: 0 15px 35px rgba(14, 165, 233, 0.15),
                  inset 0 1px 1px rgba(255, 255, 255, 0.9);
      border: 1px solid rgba(255, 255, 255, 0.8);
      width: 100%;
    }

    .card.active {
      display: block;
      animation: fadeIn 0.5s cubic-bezier(0.16, 1, 0.3, 1) forwards;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px) scale(0.96); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }

    .envelope-card {
      background: rgba(255, 255, 255, 0.94);
      border-radius: 24px;
      padding: 35px 20px;
      text-align: center;
      cursor: pointer;
      box-shadow: 0 15px 35px rgba(2, 132, 199, 0.15);
      border: 2px dashed #7dd3fc;
      transition: all 0.3s ease;
    }

    .envelope-card:hover {
      transform: translateY(-5px);
    }

    .envelope-icon {
      font-size: 4.5rem;
      margin-bottom: 10px;
      display: inline-block;
      animation: pulseHeart 1.5s infinite alternate;
    }

    @keyframes pulseHeart {
      0% { transform: scale(1); }
      100% { transform: scale(1.15); }
    }

    .badge {
      display: inline-block;
      background: #e0f2fe;
      color: #0284c7;
      border: 1px solid #bae6fd;
      font-size: 0.75rem;
      font-weight: 700;
      padding: 6px 14px;
      border-radius: 20px;
      margin-bottom: 12px;
      letter-spacing: 0.5px;
      text-transform: uppercase;
    }

    /* Grid Media Gambar */
    .media-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(110px, 1fr));
      gap: 10px;
      margin-bottom: 16px;
    }

    .media-frame {
      width: 100%;
      height: 120px;
      border-radius: 14px;
      overflow: hidden;
      border: 2px solid #ffffff;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
    }

    .media-frame img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    /* Video Player Frame khusus Kartu 8 */
    .video-player-frame {
      width: 100%;
      border-radius: 16px;
      overflow: hidden;
      border: 2px solid #ffffff;
      box-shadow: 0 8px 20px rgba(2, 132, 199, 0.2);
      margin-bottom: 16px;
      background: #000;
    }

    .video-player-frame video {
      width: 100%;
      max-height: 250px;
      display: block;
    }

    /* Typing Box */
    .typing-box {
      background: rgba(240, 249, 255, 0.75);
      border: 1px solid #bae6fd;
      border-radius: 16px;
      padding: 18px;
      margin-bottom: 20px;
      text-align: left;
      font-size: 0.95rem;
      line-height: 1.6;
      color: #334155;
      min-height: 80px;
      position: relative;
    }

    .cursor {
      display: inline-block;
      width: 3px;
      height: 1em;
      background-color: #0284c7;
      vertical-align: middle;
      animation: blink 0.7s infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    .btn {
      background: linear-gradient(135deg, #38bdf8 0%, #0284c7 100%);
      color: white;
      border: none;
      padding: 13px 24px;
      border-radius: 50px;
      font-weight: 600;
      font-size: 0.9rem;
      cursor: pointer;
      box-shadow: 0 6px 18px rgba(2, 132, 199, 0.25);
      transition: all 0.2s ease;
      width: 100%;
    }

    .btn:active { transform: scale(0.97); }

    .click-sparkle {
      position: fixed;
      border-radius: 50%;
      background: #ffffff;
      box-shadow: 0 0 10px #ffffff, 0 0 20px #38bdf8;
      pointer-events: none;
      animation: floatUpSparkle 1.6s cubic-bezier(0.25, 1, 0.5, 1) forwards;
      z-index: 10;
    }

    @keyframes floatUpSparkle {
      0% { opacity: 1; transform: translate(0, 0) scale(1); }
      100% { opacity: 0; transform: translate(var(--tw-x), -100px) scale(0.2); }
    }

    .music-control {
      position: fixed;
      top: 16px;
      right: 16px;
      z-index: 100;
      background: rgba(255, 255, 255, 0.85);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.9);
      width: 42px;
      height: 42px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      font-size: 1.2rem;
    }
  </style>
</head>
<body>

  <audio id="bgMusic" loop>
    <source src="musik.mp3" type="audio/mpeg">
  </audio>

  <button class="music-control" id="musicBtn" onclick="toggleMusic()">🎵</button>

  <div class="light-glow glow-1"></div>
  <div class="light-glow glow-2"></div>
  <div class="bg-sparkle-container" id="bgSparkleContainer"></div>

  <div class="wrapper">

    <!-- KARTU 1: SURAT DEPAN -->
    <div class="card envelope-card active" id="cardEnvelope" onclick="openEnvelope(event)">
      <span class="badge">A Special Letter For You 💌</span>
      <div class="envelope-icon">💌</div>
      <p style="margin-top: 8px; font-size: 0.85rem; color: #0284c7; font-weight: 600;">
        Klik Disini✨
      </p>
    </div>

    <!-- KARTU 2 -->
    <div class="card" id="card2">
      <div class="typing-box">
        <span id="typeText2"></span><span class="cursor" id="cursor2"></span>
      </div>
      <button class="btn" onclick="nextCard('card2', 'card3', event)">Lanjut... ✨</button>
    </div>

    <!-- KARTU 3 -->
    <div class="card" id="card3">
      <div class="typing-box">
        <span id="typeText3"></span><span class="cursor" id="cursor3"></span>
      </div>
      <button class="btn" onclick="nextCard('card3', 'card4', event)">Lanjut... ✨</button>
    </div>

    <!-- KARTU 4 -->
    <div class="card" id="card4">
      <div class="typing-box">
        <span id="typeText4"></span><span class="cursor" id="cursor4"></span>
      </div>
      <button class="btn" onclick="nextCard('card4', 'card5', event)">Lanjut... ✨</button>
    </div>

    <!-- KARTU 5 -->
    <div class="card" id="card5">
      <div class="typing-box">
        <span id="typeText5"></span><span class="cursor" id="cursor5"></span>
      </div>
      <button class="btn" onclick="nextCard('card5', 'card6', event)">Lanjut... ✨</button>
    </div>

    <!-- KARTU 6 -->
    <div class="card" id="card6">
      <div class="typing-box">
        <span id="typeText6"></span><span class="cursor" id="cursor6"></span>
      </div>
      <button class="btn" onclick="nextCard('card6', 'card7', event)">Lanjut... ✨</button>
    </div>

    <!-- KARTU 7 -->
    <div class="card" id="card7">
      <div class="typing-box">
        <span id="typeText7"></span><span class="cursor" id="cursor7"></span>
      </div>
      <button class="btn" onclick="nextCard('card7', 'card8', event)">Tonton Vidio Spesial 🎬</button>
    </div>

    <!-- KARTU 8: PEMUTAR VIDEO (OTOMATIS PINDAH SAAT SELESAI) -->
    <div class="card" id="card8">
      <span class="badge">Special Video For You 🎬</span>
      <div class="video-player-frame">
        <video id="specialVideo" controls playsinline>
          <source src="video1.mp4" type="video/mp4">
          Browser kamu tidak mendukung pemutaran video.
        </video>
      </div>
      <p style="font-size: 0.8rem; color: #64748b; margin-bottom: 12px;">
        *Video akan selesai dan otomatis lanjut ke surat tulisan tangan ✨
      </p>
      <button class="btn" onclick="skipVideo(event)">Lewati Video ⏭️</button>
    </div>

  <script>
    // --- TEKS SINGKAT KARTU 2 - 7 ---
    const text2 = "alowwww";
    const text3 = "long time no see sayang";
    const text4 = "long time no greeting.... anjai";
    const text5 = "lebay yakan. baru berapa hari";
    const text6 = "aku ganggu waktunya bentar yaaaa";
    const text7 = "mau yapping dulu";

    // Music Engine
    const music = document.getElementById('bgMusic');
    const musicBtn = document.getElementById('musicBtn');
    let isMusicPlaying = false;

    function toggleMusic() {
      if (isMusicPlaying) {
        music.pause();
        musicBtn.innerText = '🔇';
        isMusicPlaying = false;
      } else {
        music.play();
        musicBtn.innerText = '🎵';
        isMusicPlaying = true;
      }
    }

    function playMusicAuto() {
      if (!isMusicPlaying) {
        music.play().then(() => {
          isMusicPlaying = true;
          musicBtn.innerText = '🎵';
        }).catch(err => console.log("Autoplay blocked: " + err));
      }
    }

    // Typing Engine
    let currentTimeout = null;
    function typeEffect(elementId, cursorId, text, speed = 35) {
      const el = document.getElementById(elementId);
      const cursor = document.getElementById(cursorId);
      el.innerHTML = "";
      cursor.style.display = "inline-block";
      
      let i = 0;
      function typing() {
        if (i < text.length) {
          if (text.charAt(i) === "\n") {
            el.innerHTML += "<br>";
          } else {
            el.innerHTML += text.charAt(i);
          }
          i++;
          currentTimeout = setTimeout(typing, speed);
        } else {
          cursor.style.display = "none";
        }
      }
      typing();
    }

    function openEnvelope(e) {
      playMusicAuto();
      document.getElementById('cardEnvelope').classList.remove('active');
      document.getElementById('card2').classList.add('active');
      typeEffect('typeText2', 'cursor2', text2);
      createClickSparkles(e);
    }

    const specialVideo = document.getElementById('specialVideo');

    function nextCard(currentId, nextId, e) {
      playMusicAuto();
      clearTimeout(currentTimeout);
      document.getElementById(currentId).classList.remove('active');
      document.getElementById(nextId).classList.add('active');
      createClickSparkles(e);

      // Logika Typing Per Kartu
      if (nextId === 'card2') typeEffect('typeText2', 'cursor2', text2);
      else if (nextId === 'card3') typeEffect('typeText3', 'cursor3', text3);
      else if (nextId === 'card4') typeEffect('typeText4', 'cursor4', text4);
      else if (nextId === 'card5') typeEffect('typeText5', 'cursor5', text5);
      else if (nextId === 'card6') typeEffect('typeText6', 'cursor6', text6);
      else if (nextId === 'card7') typeEffect('typeText7', 'cursor7', text7);
      else if (nextId === 'card8') {
        // Matikan musik latar belakang sementara video diputar
        if (isMusicPlaying) {
          music.pause();
        }
        specialVideo.currentTime = 0;
        specialVideo.play().catch(err => console.log("Video auto play blocked: " + err));
      } else if (nextId === 'cardPart1') {
        // Nyalakan kembali musik latar belakang jika sebelumnya aktif
        if (isMusicPlaying) {
          music.play();
        }
        typeEffect('typeTextPart1', 'cursorPart1', textPart1);
      } else if (nextId === 'cardPart2') typeEffect('typeTextPart2', 'cursorPart2', textPart2);
      else if (nextId === 'cardPart3') typeEffect('typeTextPart3', 'cursorPart3', textPart3);
      else if (nextId === 'cardPart4') typeEffect('typeTextPart4', 'cursorPart4', textPart4);
      else if (nextId === 'cardFinal') typeEffect('typeTextPart5', 'cursorPart5', textPart5);
    }

    // Event ketika durasi video selesai, langsung lanjut otomatis ke Kartu 9 (cardPart1)
    specialVideo.onended = function() {
      document.getElementById('card8').classList.remove('active');
      document.getElementById('cardPart1').classList.add('active');
      if (isMusicPlaying) {
        music.play();
      }
      typeEffect('typeTextPart1', 'cursorPart1', textPart1);
    };

    function skipVideo(e) {
      specialVideo.pause();
      nextCard('card8', 'cardPart1', e);
    }

    function restartCards(e) {
      clearTimeout(currentTimeout);
      specialVideo.pause();
      document.querySelectorAll('.card').forEach(card => card.classList.remove('active'));
      document.getElementById('cardEnvelope').classList.add('active');
      createClickSparkles(e);
    }

    function createBgSparkles() {
      const container = document.getElementById('bgSparkleContainer');
      for (let i = 0; i < 25; i++) {
        const sparkle = document.createElement('div');
        sparkle.classList.add('floating-bg-sparkle');
        sparkle.style.left = Math.random() * 100 + '%';
        const size = (Math.random() * 8 + 4) + 'px';
        sparkle.style.width = size;
        sparkle.style.height = size;
        sparkle.style.setProperty('--duration', (Math.random() * 6 + 6) + 's');
        sparkle.style.setProperty('--delay', (Math.random() * 8) + 's');
        container.appendChild(sparkle);
      }
    }
    createBgSparkles();

    function createClickSparkles(e) {
      for (let i = 0; i < 12; i++) {
        const sparkle = document.createElement('div');
        sparkle.classList.add('click-sparkle');
        const size = (Math.random() * 8 + 5) + 'px';
        sparkle.style.width = size;
        sparkle.style.height = size;
        sparkle.style.left = e.clientX + 'px';
        sparkle.style.top = e.clientY + 'px';
        sparkle.style.setProperty('--tw-x', (Math.random() * 100 - 50) + 'px');
        document.body.appendChild(sparkle);
        setTimeout(() => sparkle.remove(), 1600);
      }
    }
  </script>
</body>
</html>
