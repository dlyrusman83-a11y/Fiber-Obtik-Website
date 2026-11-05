<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FiberPro - Jasa Fiber Optik</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background: #0b1120;
      color: white;
      line-height: 1.6;
    }

    header {
      padding: 20px 8%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #111827;
    }

    .logo {
      color: #38bdf8;
      font-size: 23px;
      font-weight: bold;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 15px;
    }

    .hero {
      padding: 80px 8%;
      text-align: center;
      background: linear-gradient(135deg, #0f172a, #075985);
    }

    .hero h1 {
      font-size: 36px;
      margin-bottom: 15px;
    }

    .hero p {
      color: #dbeafe;
      margin-bottom: 25px;
    }

    .btn {
      display: inline-block;
      background: #22c55e;
      color: white;
      padding: 12px 24px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 50px 8%;
      text-align: center;
    }

    h2 {
      margin-bottom: 25px;
      color: #38bdf8;
    }

    .layanan {
      display: grid;
      grid-template-columns: repeat(
        auto-fit, minmax(220px, 1fr)
      );
      gap: 20px;
    }

    .card {
      background: #1e293b;
      padding: 25px;
      border-radius: 12px;
      border: 1px solid #334155;
    }

    .card h3 {
      margin-bottom: 12px;
      color: #7dd3fc;
    }

    .harga {
      font-size: 22px;
      font-weight: bold;
      color: #4ade80;
      margin: 15px 0;
    }

    .kontak {
      background: #111827;
    }

    footer {
      padding: 20px;
      text-align: center;
      color: #94a3b8;
    }

    @media (max-width: 600px) {
      .hero h1 {
        font-size: 28px;
      }

      nav a {
        margin-left: 8px;
        font-size: 13px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">FiberPro</div>
    <nav>
      <a href="#layanan">Layanan</a>
      <a href="#harga">Harga</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </header>

  <div class="hero">
    <h1>Jasa Pemasangan Fiber Optik</h1>
    <p>
      Solusi instalasi jaringan fiber optik
      untuk rumah, kantor, dan usaha.
    </p>
    <a class="btn"
       href="https://wa.me/6281234567890">
      Pesan Sekarang
    </a>
  </div>

  <section id="layanan">
    <h2>Layanan Kami</h2>

    <div class="layanan">
      <div class="card">
        <h3>Instalasi Fiber Optik</h3>
        <p>Pemasangan kabel fiber optik untuk jaringan internet.</p>
      </div>

      <div class="card">
        <h3>Splicing Fiber Optik</h3>
        <p>Penyambungan kabel fiber optik menggunakan alat khusus.</p>
      </div>

      <div class="card">
        <h3>Perbaikan Jaringan</h3>
        <p>Pemeriksaan dan perbaikan gangguan jaringan fiber optik.</p>
      </div>
    </div>
  </section>

  <section id="harga">
    <h2>Daftar Harga</h2>

    <div class="layanan">
      <div class="card">
        <h3>Pemasangan Rumah</h3>
        <p>Instalasi jaringan untuk rumah atau kos.</p>
        <div class="harga">Mulai Rp150.000</div>
      </div>

      <div class="card">
        <h3>Splicing Kabel</h3>
        <p>Penyambungan kabel fiber optik.</p>
        <div class="harga">Mulai Rp50.000</div>
      </div>

      <div class="card">
        <h3>Survey Lokasi</h3>
        <p>Pengecekan lokasi sebelum pemasangan.</p>
        <div class="harga">Hubungi Kami</div>
      </div>
    </div>

    <p style="margin-top:20px;color:#94a3b8">
      Harga di atas hanya contoh. Sesuaikan dengan
      tarif dan wilayah layanan Anda.
    </p>
  </section>

  <section id="kontak" class="kontak">
    <h2>Hubungi Kami</h2>
    <p>Butuh pemasangan fiber optik? Konsultasikan kebutuhan Anda.</p>
    <br>

    <a class="btn"
       href="https://wa.me/6281234567890?text=Halo%2C%20saya%20ingin%20memesan%20jasa%20fiber%20optik">
      Chat WhatsApp
    </a>
  </section>

  <footer>
    <p>© 2026 FiberPro | Jasa Fiber Optik</p>
  </footer>

</body>
</html>
