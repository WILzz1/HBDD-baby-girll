
<html lang="id">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Ucapan Ulang Tahun</title>
  <!-- Bootstrap 5 -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{--accent:#ff597b;--accent-2:#ffb86b}
    body{font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial; background: linear-gradient(135deg,#fff7fb 0%, #f5faff 40%, #fffef6 100%);}
    .hero{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:3rem 1rem}
    .card-hero{border-radius:20px;box-shadow:0 10px 30px rgba(13,30,59,0.08);overflow:hidden}
    .left{background:linear-gradient(180deg, rgba(255,89,123,0.08), rgba(255,184,107,0.06));padding:2.5rem}
    .right{background:radial-gradient(circle at 10% 10%, #fff, #f7fbff);padding:2.5rem}
    h1{color:#0c2a43;font-weight:800;letter-spacing:0.2px}
    p.lead{font-size:1.05rem;color:#24475a}
    .heart{width:100px;height:90px;position:relative;margin:10px auto}
    .heart:before,.heart:after{content:"";position:absolute;left:50px;top:0;width:50px;height:80px;background:var(--accent);border-radius:50px 50px 0 0;transform:rotate(-45deg);transform-origin:0 100%}
    .heart:after{left:0;transform:rotate(45deg);transform-origin:100% 100%}
    .pulse{animation:pulse 1.6s infinite}
    @keyframes pulse{0%{transform:scale(1)}50%{transform:scale(1.08)}100%{transform:scale(1)}}
    .balloon{position:absolute;bottom:-40px;opacity:0.95}
    .balloon.b1{left:10%;animation:float 6s ease-in-out infinite}
    .balloon.b2{left:40%;animation:float 5.5s ease-in-out 0.3s infinite}
    .balloon.b3{left:70%;animation:float 6.7s ease-in-out 0.6s infinite}
    @keyframes float{0%{transform:translateY(0)}50%{transform:translateY(-18px)}100%{transform:translateY(0)}}
    .small{font-size:0.88rem;color:#5a6b74}
    .btn-accent{background:linear-gradient(90deg,var(--accent),var(--accent-2));border:none;color:white}
    .footer-note{font-size:0.82rem;color:#7a8a94}
    @media (max-width:767px){.card-hero{border-radius:14px}.left,.right{padding:1.25rem}}
  </style>
</head>
<body>
  <div class="hero container">
    <div class="card card-hero row g-0 align-items-stretch">
      <div class="col-md-6 left position-relative">
        <!-- decorative balloons -->
        <svg class="balloon b1" width="90" height="140" viewBox="0 0 90 140" fill="none" xmlns="http://www.w3.org/2000/svg">
          <ellipse cx="45" cy="50" rx="36" ry="44" fill="#ffb86b"/>
          <path d="M45 94 L45 120" stroke="#d97a3b" stroke-width="2" stroke-linecap="round"/>
        </svg>
        <svg class="balloon b2" width="70" height="110" viewBox="0 0 70 110" fill="none" xmlns="http://www.w3.org/2000/svg">
          <ellipse cx="35" cy="40" rx="28" ry="34" fill="#ff597b"/>
          <path d="M35 74 L35 96" stroke="#b93b57" stroke-width="2" stroke-linecap="round"/>
        </svg>
        <svg class="balloon b3" width="80" height="120" viewBox="0 0 80 120" fill="none" xmlns="http://www.w3.org/2000/svg">
          <ellipse cx="40" cy="44" rx="32" ry="38" fill="#ffd1ea"/>
          <path d="M40 84 L40 110" stroke="#e49db9" stroke-width="2" stroke-linecap="round"/>
        </svg>

        <div class="d-flex flex-column h-100 justify-content-center">
          <div class="text-center mb-3">
            <div class="heart pulse" aria-hidden="true"></div>
            <h1 class="mb-0">Selamat Ulang Tahun</h1>
            <p class="small mt-1">Untuk yang tersayang 💖</p>
          </div>

          <div class="text-center">
            <p class="lead">Hai <span id="toNameDisplay" style="font-weight:700">Sayang</span> — maaf aku kirim nya telat ya sayaang, aku sangat bahagiaa ada kamu disini. Mendengar suara mu saja aku sangat bahagia,mau keadaan kamu gimanapun aku akan selalu ada buat kamu sayaang.</p>
            <p id="kesanDisplay" class="small mt-2">Terima kasih sudah hadir dan bertahan bersamaku hingga sejauh ini 💖</p>
            <p class="small">[IqlimaArjasariAsa]</p>
            <p class="small" style="font-weight:700">[From: Satriawily]</p>

            <div class="mt-4 d-flex justify-content-center gap-2">
              <button class="btn btn-accent" id="btnSurprise">Kirim Kejutan</button>
              <button class="btn btn-outline-primary" id="btnEdit">Edit Nama</button>
            </div>
          </div>
        </div>

      </div>
      <div class="col-md-6 right d-flex flex-column justify-content-center">
        <div class="container">
          <h5 class="mb-3">Personalisasi</h5>

          <form id="formPersonal">
            <div class="mb-3">
              <label for="toName" class="form-label">Untuk (Orang paling cantik sedunia)</label>
              <input type="text" class="form-control" id="toName" placeholder="Masukkan nama..." value="IqlimaArjasariAsa">
            </div>
            <div class="mb-3">
              <label for="fromName" class="form-label">Dari (Orang paling ganteng sedunia)</label>
              <input type="text" class="form-control" id="fromName" placeholder="Namamu..." value="Satriawily">
            </div>
            <div class="mb-3">
              <label for="customMsg" class="form-label">Pesan Singkat</label>
              <textarea id="customMsg" class="form-control" rows="3">semoga lekas sembuh ya sayaang, maaf jika aku sering buat salah,aku sangat bahagia ada kamuu yang selalu menemani ku setiap saat makasih ya cintaaa ❤️</textarea>
            </div>
            <div class="mb-3">
              <label for="kesanMsg" class="form-label">Kesan & Pesan</label>
              <textarea id="kesanMsg" class="form-control" rows="3">Terima kasih sudah hadir dan bertahan bersamaku hingga sejauh ini, mau keadaan mu seperti apa aku gak peduli aku akan tetep sama kamu cinta,makasih banyak udah adaa buat akuu aku sangatt bahagiaa ya cinta kuu 💖</textarea>
            </div>
            <div class="d-flex gap-2">
              <button type="button" id="btnApply" class="btn btn-primary">Terapkan</button>
              <button type="button" id="btnReset" class="btn btn-outline-secondary">Reset</button>
            </div>
          </form>

          <hr>
          <p class="footer-note">Tips: tekan "Kirim Kejutan" untuk menampilkan pesan spesial. Gunakan tombol Edit Nama untuk mengganti nama cepat.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Optional JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
  <script>
    // Simple interactivity: apply personalization and show a mini 'surprise' animation
    const toNameInput = document.getElementById('toName');
    const fromNameInput = document.getElementById('fromName');
    const customMsgInput = document.getElementById('customMsg');
    const kesanMs
    const toNameDisplay = document.getElementById('toNameDisplay');
    const btnApply = document.getElementById('btnApply');
    const btnReset = document.getElementById('btnReset');
    const btnSurprise = document.getElementById('btnSurprise');
    const btnEdit = document.getElementById('btnEdit');

    btnApply.addEventListener('click', ()=>{
      const to = toNameInput.value.trim() || 'Sayang';
      const from = fromNameInput.value.trim() || '[Nama Kamu]';
      const msg = customMsgInput.value.trim() || '';
      toNameDisplay.textContent = to;
      // update main message
      document.querySelector('.lead').textContent = msg || `Hai ${to} — semoga hari ini penuh tawa, kue, dan pelukan hangat. Terima kasih sudah jadi alasan kecilku bahagia setiap hari.`;
      // update sign
      document.querySelectorAll('.small')[1].textContent = from;
    });

    btnReset.addEventListener('click', ()=>{
      toNameInput.value = 'Sayang';
      fromNameInput.value = '[Nama Kamu]';
      customMsgInput.value = 'Semoga semua keinginanmu terkabul. Aku sayang kamu ❤️';
      btnApply.click();
    });

    btnEdit.addEventListener('click', ()=>{ toNameInput.focus(); });

    // Simple confetti effect (small and dependency-free)
    function makeConfetti() {
      const count = 24;
      for (let i=0;i<count;i++){
        const el = document.createElement('div');
        el.style.position = 'fixed';
        el.style.left = Math.random()*100 + '%';
        el.style.top = '-10px';
        el.style.width = el.style.height = Math.floor(Math.random()*8)+6 + 'px';
        el.style.background = ['#ff597b','#ffb86b','#ffd1ea','#6bd3ff'][Math.floor(Math.random()*4)];
        el.style.opacity = '0.95';
        el.style.transform = `rotate(${Math.random()*360}deg)`;
        el.style.borderRadius = '2px';
        el.style.zIndex = 9999;
        const fall = 2000 + Math.random()*1800;
        document.body.appendChild(el);
        el.animate([
          {transform: 'translateY(0) rotate(0deg)', opacity:1},
          {transform: `translateY(${window.innerHeight + 200}px) rotate(${Math.random()*720}deg)`, opacity:0.9}
        ],{duration:fall, easing:'cubic-bezier(.2,.8,.2,1)'}).onfinish = ()=> el.remove();
      }
    }

    btnSurprise.addEventListener('click', ()=>{
      makeConfetti();
      // flash the heart
      const heart = document.querySelector('.heart');
      heart.style.transform = 'scale(1.12)';
      setTimeout(()=>heart.style.transform = '', 450);
    });

    // initialize defaults
    document.addEventListener('DOMContentLoaded', ()=>{
      document.getElementById('btnReset').click();
    });
  </script>
</body>
</html>
