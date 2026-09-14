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

    /* Pattern Kaligrafi di Background */
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-image: radial-gradient(rgba(56, 189, 248, 0.15) 1px, transparent 0),
                        url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200' viewBox='0 0 200 200'%3E%3Cpath fill='none' stroke='%230284c7' stroke-width='1.5' opacity='0.08' d='M35.5,45.5 C40,20 70,20 80,40 C90,60 60,80 50,95 C40,110 70,120 85,100 C100,80 90,50 110,40 C130,30 150,60 135,80 C120,100 150,130 170,110'/%3E%3Ctext x='20' y='140' font-family='serif' font-style='italic' font-size='22' fill='%230284c7' opacity='0.06'%3EAesthetic Calligraphy✨%3C/text%3E%3C/svg%3E");
      background-size: 100px 100px, 250px 250px;
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
      max-width: 420px;
      z-index: 2;
      margin: 20px 0;
    }

    .card {
      display: none;
      background: rgba(255, 255, 255, 0.9);
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
      background: rgba(255, 255, 255, 0.92);
      border-radius: 24px;
      padding: 30px 20px;
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

    /* Multi-media Container (Grid Foto/Video) */
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

    .media-frame img, .media-frame video {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    /* Teks Ketik (Typing Text Styling) */
    .typing-box {
      background: rgba(240, 249, 255, 0.7);
      border: 1px solid #bae6fd;
      border-radius: 16px;
      padding: 16px;
      margin-bottom: 20px;
      text-align: left;
      font-size: 0.9rem;
      line-height: 1.6;
      color: #334155;
      min-height: 100px;
      position: relative;
    }

    /* Kursor Berkedip */
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

    /* KALENDER STYLING */
    .calendar-box {
      background: #ffffff;
      border-radius: 16px;
      padding: 16px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
      margin-bottom: 20px;
      border: 1px solid #e0f2fe;
    }

    .calendar-header {
      font-weight: 700;
      color: #0284c7;
      font-size: 1.1rem;
      margin-bottom: 12px;
    }

    .calendar-grid {
      display: grid;
      grid-template-columns: repeat(7, 1fr);
      gap: 6px;
      text-align: center;
      font-size: 0.85rem;
    }

    .day-name {
      font-weight: 600;
      color: #64748b;
      font-size: 0.75rem;
      padding-bottom: 4px;
    }

    .day-num {
      padding: 8px 0;
      color: #334155;
      border-radius: 50%;
    }

    .day-num.empty { visibility: hidden; }

    .day-num.birthday {
      background: #e0f2fe;
      color: #0284c7;
      font-weight: 800;
      border: 2px solid #38bdf8;
      animation: popBirthday 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275) infinite alternate;
    }

    @keyframes popBirthday {
      0% { transform: scale(1); }
      100% { transform: scale(1.12); box-shadow: 0 0 12px rgba(56, 189, 248, 0.5); }
    }

    .card h2 {
      font-size: 1.3rem;
      font-weight: 700;
      color: #0f172a;
      margin-bottom: 10px;
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

    <!-- SURAT DEPAN -->
    <div class="card envelope-card active" id="cardEnvelope" onclick="openEnvelope(event)">
      <span class="badge">A Special Letter For You 💌</span>
      <div class="envelope-icon">💌</div>
      <p style="margin-top: 8px; font-size: 0.85rem; color: #0284c7; font-weight: 600;">
        Klik Disini✨
      </p>
    </div>

    <!-- KARTU 1: KALENDER -->
    <div class="card" id="cardCalendar">
      <span class="badge">A Very Special Day 🗓️</span>
      <div class="calendar-box">
        <div class="calendar-header">September 2026 💖</div>
        <div class="calendar-grid">
          <div class="day-name">Min</div><div class="day-name">Sen</div><div class="day-name">Sel</div>
          <div class="day-name">Rab</div><div class="day-name">Kam</div><div class="day-name">Jum</div><div class="day-name">Sab</div>

          <div class="day-num empty"></div><div class="day-num empty"></div>
          <div class="day-num">1</div><div class="day-num">2</div><div class="day-num">3</div><div class="day-num">4</div><div class="day-num">5</div>
          <div class="day-num">6</div><div class="day-num">7</div><div class="day-num">8</div><div class="day-num">9</div><div class="day-num">10</div>
          <div class="day-num">11</div><div class="day-num">12</div><div class="day-num">13</div><div class="day-num">14</div><div class="day-num">15</div>
          <div class="day-num">16</div><div class="day-num">17</div><div class="day-num">18</div><div class="day-num">19</div><div class="day-num">20</div>
          <div class="day-num">21</div><div class="day-num">22</div>
          <div class="day-num birthday">23 🎂</div>
          <div class="day-num">24</div><div class="day-num">25</div><div class="day-num">26</div><div class="day-num">27</div><div class="day-num">28</div>
          <div class="day-num">29</div><div class="day-num">30</div><div class="day-num">31</div>
        </div>
      </div>
      <h2>Hari Spesial Partnerku! 🥳</h2>
      <button class="btn" onclick="nextCard('cardCalendar', 'cardWish', event)">Buka Pesan Pertama ✨</button>
    </div>

    <!-- KARTU 2: UCAPAN & KENANGAN (FOTO + VIDEO + UCAPAN KETIK PANJANG) -->
    <div class="card" id="cardWish">
      <span class="badge">Happy Birthday Sayang! 🎂</span>
      
      <!-- Muat 3 Foto/Video Sekaligus dalam 1 Kartu -->
      <div class="media-grid">
        <div class="media-frame"><img src="foto1.jpeg" alt="Foto 1"></div>
        <div class="media-frame"><img src="foto2.jpeg" alt="Foto 2"></div>
        <div class="media-frame">
          <!-- Bisa ganti src jadi video.mp4 jika pakai video -->
          <video autoplay loop muted playsinline>
            <source src="video1.mp4" type="video/mp4">
            <img src="foto7.jpeg" alt="Fallback Foto">
          </video>
        </div>
      </div>

      <!-- Kotak Teks Yang Berjalan/Ketik Otomatis -->
      <div class="typing-box">
        <span id="typeText1"></span><span class="cursor" id="cursor1"></span>
      </div>

      <button class="btn" onclick="nextCard('cardWish', 'cardDeepMessage', event)">Lanjut ke Pesan Hati 💙</button>
    </div>

    <!-- KARTU 3: PESAN MENDALAM (BANYAK FOTO + TEKS KETIK) -->
    <div class="card" id="cardDeepMessage">
      <span class="badge">Terima Kasih & Maaf ✨</span>
      
      <!-- Muat Banyak Foto Lagi -->
      <div class="media-grid">
        <div class="media-frame"><img src="foto4.jpeg" alt="Foto 4"></div>
        <div class="media-frame"><img src="foto6.jpeg" alt="Foto 5"></div>
        <div class="media-frame"><img src="foto8.jpeg" alt="Foto 6"></div>
      </div>

      <!-- Teks Ketik Otomatis Kartu 3 -->
      <div class="typing-box">
        <span id="typeText2"></span><span class="cursor" id="cursor2"></span>
      </div>

      <button class="btn" onclick="nextCard('cardDeepMessage', 'cardFinal', event)">Pesan Terakhir 💌</button>
    </div>

    <!-- KARTU 4: PENUTUP / FINAL -->
    <div class="card" id="cardFinal">
      <span class="badge">Plot Twist & Kangen 💖</span>
      
      <div class="media-grid" style="grid-template-columns: 1fr 1fr;">
        <div class="media-frame" style="height: 150px;"><img src="foto9.jpeg" alt="Foto 7"></div>
        <div class="media-frame" style="height: 150px;"><img src="foto5.jpeg" alt="Foto 8"></div>
      </div>

      <div class="typing-box">
        <span id="typeText3"></span><span class="cursor" id="cursor3"></span>
      </div>

      <button class="btn" onclick="restartCards(event)">Ulang Dari Awal 🔄</button>
    </div>

  </div>

  <script>
    // --- TEKS YANG AKAN DIKETIK OTOMATIS (Bisa Kamu Ubah Sesuai Keinginan) ---
    const textKartu2 = "Selamat ulang tahun Sayangkuu!!🥳🎉 Partner tanggal lahirkuuu...\n\nTerima kasih ya sudah selalu membawa kenyamanan, keceriaan, dan kepercayaan di setiap momen LDR kita ini. Semoga di usia yang sekarang, segala keinginan lancar, sehat selalu, dan bahagia terus sama aku! 💙";

    const textKartu3 = "Makasi ya udah selalu baik samaku dan selalu sabar ngasi tau aku yang kadang susah berubah ini. Maaf ya kalau aku belum bisa nyampein rasa sayangku dengan sempurna sampai bikin kamu merasa sendirian.\n\nKalau nurut egoisku sih aku doa kamu gak laku-laku hehe, biar bisa tetap sama awak terus! 🤪";

    const textKartu4 = "Titip kangen di sini dulu ya!! Kartunya emang gak bisa meluk, tapi nanti ganti peluknya kalau syudah pulang dan ketemu langsung! 😉\n\nLove You So Much Sayanggg! 💖✨";

    // Global Vars Music
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

    // Function Typing Effect
    let currentTimeout = null;
    function typeEffect(elementId, cursorId, text, speed = 40) {
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
          cursor.style.display = "none"; // Sembunyikan kursor saat selesai
        }
      }
      typing();
    }

    function openEnvelope(e) {
      playMusicAuto();
      document.getElementById('cardEnvelope').classList.remove('active');
      document.getElementById('cardCalendar').classList.add('active');
      createClickSparkles(e);
    }

    function nextCard(currentId, nextId, e) {
      playMusicAuto();
      clearTimeout(currentTimeout);
      document.getElementById(currentId).classList.remove('active');
      document.getElementById(nextId).classList.add('active');
      createClickSparkles(e);

      // Triggers Typing Effect saat kartu dibuka
      if (nextId === 'cardWish') {
        typeEffect('typeText1', 'cursor1', textKartu2);
      } else if (nextId === 'cardDeepMessage') {
        typeEffect('typeText2', 'cursor2', textKartu3);
      } else if (nextId === 'cardFinal') {
        typeEffect('typeText3', 'cursor3', textKartu4);
      }
    }

    function restartCards(e) {
      clearTimeout(currentTimeout);
      document.querySelectorAll('.card').forEach(card => card.classList.remove('active'));
      document.getElementById('cardEnvelope').classList.add('active');
      createClickSparkles(e);
    }

    // Partikel Background & Click
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
