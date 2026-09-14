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

    /* Grid Media Gambar/Video */
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

    /* Typing Box */
    .typing-box {
      background: rgba(240, 249, 255, 0.75);
      border: 1px solid #bae6fd;
      border-radius: 16px;
      padding: 18px;
      margin-bottom: 20px;
      text-align: left;
      font-size: 0.9rem;
      line-height: 1.6;
      color: #334155;
      min-height: 120px;
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

    /* Kalender */
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

    <!-- AMPLOP SURAT DEPAN -->
    <div class="card envelope-card active" id="cardEnvelope" onclick="openEnvelope(event)">
      <span class="badge">Surat Ke 2 dan Terakhir 💌</span>
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
      <h2>Yapping Time... ✨</h2>
      <button class="btn" onclick="nextCard('cardCalendar', 'cardPart1', event)">Mulai Baca 💌</button>
    </div>

    <!-- KARTU 2: PEMBUKAAN (FOTO 1, 2) -->
    <div class="card" id="cardPart1">
      <span class="badge">Bagian 1 • Pembukaan</span>
      <div class="media-grid">
        <div class="media-frame"><img src="foto1.jpeg" alt="Foto 1"></div>
        <div class="media-frame"><img src="foto2.jpeg" alt="Foto 2"></div>
      </div>

      <div class="typing-box">
        <span id="typeText1"></span><span class="cursor" id="cursor1"></span>
      </div>

      <button class="btn" onclick="nextCard('cardPart1', 'cardPart2', event)">Lanjut Baca...</button>
    </div>

    <!-- KARTU 3: CERITA & PERASAAN (FOTO 3, 4, 5) -->
    <div class="card" id="cardPart2">
      <span class="badge">Bagian 2 • Kenangan & Belajar</span>
      <div class="media-grid">
        <div class="media-frame"><img src="foto3.jpeg" alt="Foto 3"></div>
        <div class="media-frame"><img src="foto4.jpeg" alt="Foto 4"></div>
        <div class="media-frame"><img src="foto5.jpeg" alt="Foto 5"></div>
      </div>

      <div class="typing-box">
        <span id="typeText2"></span><span class="cursor" id="cursor2"></span>
      </div>

      <button class="btn" onclick="nextCard('cardPart2', 'cardPart3', event)">Lanjut Lagi...</button>
    </div>

    <!-- KARTU 4: CERITA HARI-HARI (FOTO 6, 7) -->
    <div class="card" id="cardPart3">
      <span class="badge">Bagian 3 • Cerita Hari-Hari</span>
      <div class="media-grid">
        <div class="media-frame"><img src="foto6.jpeg" alt="Foto 6"></div>
        <div class="media-frame"><img src="foto7.jpeg" alt="Foto 7"></div>
      </div>

      <div class="typing-box">
        <span id="typeText3"></span><span class="cursor" id="cursor3"></span>
      </div>

      <button class="btn" onclick="nextCard('cardPart3', 'cardPart4', event)">Masuk ke Ucapan 🎂</button>
    </div>

    <!-- KARTU 5: UCAPAN ULANG TAHUN (FOTO 8, 9) -->
    <div class="card" id="cardPart4">
      <span class="badge">Bagian 4 • Happy Birthday! 🎂</span>
      <div class="media-grid">
        <div class="media-frame"><img src="foto8.jpeg" alt="Foto 8"></div>
        <div class="media-frame"><img src="foto9.jpeg" alt="Foto 9"></div>
      </div>

      <div class="typing-box">
        <span id="typeText4"></span><span class="cursor" id="cursor4"></span>
      </div>

      <button class="btn" onclick="nextCard('cardPart4', 'cardFinal', event)">Pesan Penutup 💖</button>
    </div>

    <!-- KARTU 6: PENUTUP -->
    <div class="card" id="cardFinal">
      <span class="badge">Bagian 5 • Penutup 💙</span>
      <div class="media-grid" style="grid-template-columns: 1fr;">
        <div class="media-frame" style="height: 140px;"><img src="foto10.jpeg" alt="Foto 10"></div>
      </div>

      <div class="typing-box">
        <span id="typeText5"></span><span class="cursor" id="cursor5"></span>
      </div>

      <button class="btn" onclick="restartCards(event)">Ulang Dari Awal 🔄</button>
    </div>

  </div>

  <script>
    // --- TEKS 100% PERSIS CATATAN FOTO KAMU ---
    const textPart1 = "Long time no see, long time no greeting anjai.. hahaha\n\nMacam betul aja. Baru berapa hari. Aku ganggu bentar ya...\n\nEntah kenapa pengen buat vidio yapping untuk dia. Mau bikin web lagi sih sebenernya. Tapi adik sibuk. Tak sempat. Tada waktu lo...\n\nAku gak tau mesti mulai dari mana. Siapkan mata dan kupingnya untuk durasi panjang. Aku buat ini ditulis dulu btw. Biar enak alurnya. Pertama ni pembukaan.";

    const textPart2 = "Aku pernah bilang kan kalau aku nyesel pernah kenal sama dia. Mungkin omonganku yang itu masih terngiang-ngiang diingatannya. Tapi sebenernya bukan itu yang ku sesali. Tapi cara pertama kali kita ketemu dan memutuskan untuk kenal satu sama lain. Caranya salah.\n\nAku nyesel karna udah permainkan dia yang gak salah apa-apa, yang gak tau apa-apa. Tapi sayang, kalau boleh milih lagi, aku bakal tetap pilih untuk kenal sama dia, karena dia juga aku jadi belajar banyak hal lagi, punya cerita sama dia, pernah ngetawain hal-hal random sama dia, ngerasain gimana rasanya hubungan LDR, ngesampingin ego biar gak jadi bahan qadoh, nahan semuanya biar gak jadi pikiran dan beban dia disana.\n\nTapi ternyata caraku itu bukan cara yang bener. Hal yang ku kira bakal bisa mempertahankan hubungan kita malah jadi bom waktu dan buat kita berakhir jadi kek gini.\n\nDan sekarang, karna ulahku kita jadi asing hehe. Tapi, hidupku juga harus tetap jalan dan berlanjut. Walaupun aku harus sering nyari tempat pelarian karena rasanya setengah dari jiwaku ikut pigi sama dia.";

    const textPart3 = "Aku juga pernah bilang sama dia waktu sebelum balikan.\n\"Jangan gantungkan kepercayaan dan kebahagiaanmu pada orang lain. Karena kalau orangnya pigi, kita bakal kehilangan diri kita. Maka sisakanlah sedikit ruang ikhlas untuk diri sendiri\".\n\nTapi nyatanya, omongan tak semudah saat melakukan. Eh.. tebalek.\n\nAku kecolongan lagi, aku ngalami hal kek gini lagi di orang yang sama hehe. Tapi aku gak nyesel dan malah berterimakasih karna mau balik dan milih aku lagi walaupun waktunya sebentar.\n\nDia tau... ku pikir, dengan aku ngapus semua sosmed dia, aku bakal berenti sampe situ. Tapi nyatanya malah buat aku tambah kepo hehe. Dan gak tau kenapa asal dia masukkan vidio ke tiktok, ke ig, atau dia live pasti lewat berandaku. Kan aku jadi pengen liat. Dan.. bohong aku gak cemburu liat respon dia nanggapin komen monyet-monyet itu. Dodolkan?\n\nDan dia tau... aku mulai dinotice orang rumah. Terutama mamak. Ditanya kenapa kadang pulang sekolah kenapa sertekali, kenapa sering keluar malam sendirian. Aku bilang gak papa pengen cari angin sekalian liat orang-orang lewat sambil ngopi. Zulfi juga nanya kenapa aku sering ngajak dia keluar. Aku bilang kita putus, trus zulfi heran kenapa aku gak posting galau-galau. Gak tau aja zulfi kalau aku banjir-banjir dan berlinang ingus dikamar. Lola juga nawarin aku kenalan sama kawannya, puput juga sibuk mau nyarikan boncengan biar jadi pigi nanti. Tapi aku gak mau. Aku tetep maunya sama dia. Kalaupun gak bisa, aku bisa pigi sendiri tanpa boncengan yang lain. Munafikkan?";

    const textPart4 = "Aku masih dia nunggu pulang ke aku. Ya walaupun gak tau kapan.\n\nTapi aku gak mau meksa dan nanya-nanya lagi. Aku bakal tetap stay dibelakang dia. Kalau dia butuh aku, aku ada.\n\nAku sabar. Semalam itu jugakan kita kek gini. Asing, hidup masing-masing, punya pasangan masing-masing, tapi akhirnya juga balik lagi. Nanti juga bakal kek gitu kan sayang? Kita hanya butuh jeda lagi adakan? Nunggu dia pulang dari papua aja aku sabar. Masa nunggu dia balik ke aku, aku gak sabar. Entah aku yang terlalu ingin, atau emang masih belum terima kalau ini emang harus berenti sampe sini. Karna... aku juga gak tau ini bakal gimana. Apakah bakal tambah asing? Atau masih bisa bertegur sapa? Atau... malah cuma jadi 2 manusia yang pernah kenal satu sama lain.\n\nTapi gak papa. Aku seneng bisa jalin hubungan lagi sama dia kedua kalinya walaupun bentar doang.\n\nKadang aku bertanya-tanya. Dia lagi apa ya? Gimana kerjaannya? Sehatnya dia? Dicana udah ada hujan belum? Dia masih sering pitek gak ya? Siapa ya kawan cerita dia sekarang. Ah banyak lah.\n\nAku udah gak terlalu sedih tau... Udah gak nangis-nangis lagi... Nangis juga sih kadang. Masih mimpiin dia juga tapi. Hmm..\n\nBanyak hal yang mau ku ceritain. Saat-saat kek gini baru banyak yang mau dibagi. Dia tau... Aku nyoba daftar KAI semalam itu. Dikasi link sama pak nur orang imigrasi. Katanya bapak itu punya kenalan orang KAI. Adik juga nyoba daftar di grapari kisaran. Tau dia... malamnya daftar, paginya langsung test online. Tapi ujiannya kek eek. Gak suka.\n\nAdik juga lagi belajar bahasa Jepang sayang. Jadi opsi terakhir kalau-kalau di KAI gak diterima, habis wisuda aku masuk LPK.\n\nKawan kerja juga kek taik tau sayang. Kaget kanseng ratu melihat dunia kerja modelan kek gitu.\n\nAHH PANJANG KALI YAPPINGNYA. Selak ngantuk dia.\n\nPadahal mau ngucapin ulang tahunnya.\nSELAMAT ULANG TAHUN SAYANG...\nSehat selalu, kerjanya lancar, rezekinya lancar, segala sesuatunya dipermudah... Apalagi? Jaga diri baik-baik ya.. Jagain itu teguhku.. Jangan gatel sana sini. Jangan gatel sama sunda.";

    const textPart5 = "Kalau dengan cara kek gini dia nemuin kebahagiaan lebih, dengan cara dia live gitu dia seneng, yauda aku juga ikut seneng. Kalau dunia lagi gak baik sama dia, ingat.. aku ada di belakang dia yang selalu siap terima dia pulang.\n\nEh kapan dia cuti? Kasi-kasi kabar jugalah.. Walaupun gak bisa ketemu tapi seenggaknya aku tau dia udah disini.\n\nDan.. Semoga apa yang dia usahakan, dia upayakan bisa dia raih 1 per 1. Tapi ih... Keren kali SG dia kemaren yang spare part itu. Udah dapet arm nya ya sayang? Knalpot sama arm jadi berapa? Ih keren banget pasti itu nanti keretanya. Gak kalah keren sama yang punya. Tapi tapi.. kenapa lah buat single era. Dala sok-sok buat single era, salah pulak tulisannya- wuu-- apalah dia.\n\nDan semoga yang dia bilang mau jadi orang have ditahun depan bakal terwujud. AAMIIN--..\n\nUdah... habis. Titip salam buat orang mamak dirumah ya...\n\nALAPIYU--..\nTATA PAPAI--..";

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
    function typeEffect(elementId, cursorId, text, speed = 30) {
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
      document.getElementById('cardCalendar').classList.add('active');
      createClickSparkles(e);
    }

    function nextCard(currentId, nextId, e) {
      playMusicAuto();
      clearTimeout(currentTimeout);
      document.getElementById(currentId).classList.remove('active');
      document.getElementById(nextId).classList.add('active');
      createClickSparkles(e);

      if (nextId === 'cardPart1') {
        typeEffect('typeText1', 'cursor1', textPart1);
      } else if (nextId === 'cardPart2') {
        typeEffect('typeText2', 'cursor2', textPart2);
      } else if (nextId === 'cardPart3') {
        typeEffect('typeText3', 'cursor3', textPart3);
      } else if (nextId === 'cardPart4') {
        typeEffect('typeText4', 'cursor4', textPart4);
      } else if (nextId === 'cardFinal') {
        typeEffect('typeText5', 'cursor5', textPart5);
      }
    }

    function restartCards(e) {
      clearTimeout(currentTimeout);
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
