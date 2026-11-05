
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fiber Optik | Teknologi Masa Depan</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Arial, sans-serif;
            scroll-behavior: smooth;
        }

        :root {
            --biru-tua: #081B39;
            --biru-sedang: #143A7A;
            --teal: #22D3EE;
            --putih: #FFFFFF;
            --abu-muda: #F0F8FF;
            --abu-teks: #334155;
            --bayangan: 0 8px 24px rgba(8, 27, 57, 0.10);
        }

        body {
            background-color: var(--abu-muda);
            color: var(--abu-teks);
            line-height: 1.7;
        }

        /* Navbar */
        nav {
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 999;
            background-color: rgba(8, 27, 57, 0.92);
            backdrop-filter: blur(8px);
            padding: 16px 7%;
        }
        .nav-wrap {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            color: var(--putih);
            font-size: 24px;
            font-weight: 700;
        }
        .logo span {
            color: var(--teal);
        }
        .menu-btn {
            display: none;
            color: var(--putih);
            font-size: 30px;
            cursor: pointer;
        }
        .nav-menu {
            display: flex;
            gap: 30px;
            list-style: none;
        }
        .nav-menu li a {
            color: var(--putih);
            text-decoration: none;
            font-size: 16px;
            font-weight: 500;
            transition: 0.3s;
            position: relative;
        }
        .nav-menu li a::after {
            content: "";
            width: 0%;
            height: 2px;
            background-color: var(--teal);
            position: absolute;
            bottom: -4px;
            left: 0;
            transition: 0.3s;
        }
        .nav-menu li a:hover::after {
            width: 100%;
        }
        .nav-menu li a:hover {
            color: var(--teal);
        }

        /* Container Umum */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 5%;
        }
        section {
            padding: 80px 0;
            opacity: 0;
            transform: translateY(30px);
            animation: muncul 0.8s forwards;
        }
        section:nth-child(even) {
            animation-delay: 0.2s;
        }
        @keyframes muncul {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .judul-bagian {
            text-align: center;
            font-size: 32px;
            color: var(--biru-tua);
            margin-bottom: 50px;
        }
        .judul-bagian::after {
            content: "";
            width: 70px;
            height: 4px;
            background-color: var(--teal);
            display: block;
            margin: 10px auto 0;
            border-radius: 2px;
        }

        /* Hero Beranda */
        #beranda {
            min-height: 100vh;
            background: linear-gradient(135deg, #081B39 0%, #143A7A 60%, #164E8F 100%);
            color: var(--putih);
            display: flex;
            align-items: center;
            padding-top: 100px;
            opacity: 1;
            transform: translateY(0);
        }
        .hero-row {
            display: flex;
            gap: 50px;
            align-items: center;
            flex-wrap: wrap;
        }
        .hero-teks {
            flex: 1;
            min-width: 300px;
        }
        .hero-teks h1 {
            font-size: 46px;
            margin-bottom: 18px;
        }
        .hero-teks h1 span {
            color: var(--teal);
        }
        .hero-teks p {
            font-size: 18px;
            opacity: 0.9;
            margin-bottom: 30px;
            max-width: 580px;
        }
        .tombol-utama {
            display: inline-block;
            padding: 13px 28px;
            background-color: var(--teal);
            color: var(--biru-tua);
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: 0.3s;
            box-shadow: 0 6px 18px rgba(34, 211, 238, 0.35);
        }
        .tombol-utama:hover {
            transform: translateY(-3px);
        }
        .hero-gambar {
            flex: 1;
            min-width: 300px;
            height: 400px;
            border-radius: 20px;
            box-shadow: 0 12px 40px rgba(255,255,255,0.18);
            object-fit: cover;
        }

        /* Tentang Fiber Optik */
        #tentang {
            background-color: var(--putih);
        }
        .row-tentang {
            display: flex;
            gap: 40px;
            align-items: center;
            flex-wrap: wrap;
        }
        .gambar-tentang {
            flex: 1;
            min-width: 300px;
            height: 300px;
            border-radius: 16px;
            box-shadow: var(--bayangan);
            object-fit: cover;
        }
        .teks-tentang {
            flex: 1;
            min-width: 300px;
        }
        .teks-tentang h3 {
            font-size: 26px;
            margin-bottom: 15px;
            color: var(--biru-sedang);
        }

        /* Kelebihan */
        #kelebihan {
            background-color: var(--abu-muda);
        }
        .grid-4 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 25px;
        }
        .card {
            background-color: var(--putih);
            padding: 28px 20px;
            border-radius: 16px;
            box-shadow: var(--bayangan);
            text-align: center;
            transition: 0.3s;
        }
        .card:hover {
            transform: translateY(-6px);
        }
        .ikon-card {
            font-size: 34px;
            margin-bottom: 12px;
        }
        .card h4 {
            color: var(--biru-sedang);
            margin-bottom: 8px;
        }

        /* Jenis, Komponen, Kekurangan */
        #jenis, #komponen, #kekurangan {
            background-color: var(--putih);
        }
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }
        .card-2 {
            background-color: var(--abu-muda);
            padding: 26px;
            border-radius: 16px;
            border: 1px solid #c9e4f7;
        }
        .card-2 h3 {
            color: var(--biru-sedang);
            margin-bottom: 10px;
        }

        /* Kesimpulan Penutup */
        #kesimpulan {
            background: linear-gradient(135deg, #143A7A, #081B39);
            color: var(--putih);
        }
        #kesimpulan .judul-bagian {
            color: var(--putih);
        }
        .box-kesimpulan {
            max-width: 800px;
            margin: 0 auto;
            background-color: rgba(255,255,255,0.10);
            padding: 30px;
            border-radius: 20px;
            text-align: center;
        }

        /* Footer */
        footer {
            background-color: var(--biru-tua);
            color: var(--putih);
            text-align: center;
            padding: 24px 5%;
        }

        /* Responsif HP */
        @media (max-width: 768px) {
            .menu-btn {
                display: block;
            }
            .nav-menu {
                position: fixed;
                top: 60px;
                right: 5%;
                flex-direction: column;
                background-color: rgba(8, 27, 57, 0.96);
                width: 90%;
                padding: 20px;
                border-radius: 12px;
                display: none;
            }
            .nav-menu.aktif {
                display: flex;
            }
            .hero-teks h1 {
                font-size: 32px;
            }
            .hero-gambar {
                height: 280px;
            }
        }
    </style>
</head>
<body>
    <!-- Navbar Menu Lengkap (Tanpa Profil Kelompok) -->
    <nav>
        <div class="nav-wrap">
            <div class="logo">Fiber<span>Optik</span></div>
            <div class="menu-btn" id="menuBtn">☰</div>
            <ul class="nav-menu" id="navMenu">
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Apa Itu Fiber Optik</a></li>
                <li><a href="#kelebihan">Kelebihan</a></li>
                <li><a href="#jenis">Jenis‑Jenis</a></li>
                <li><a href="#komponen">Komponen Utama</a></li>
                <li><a href="#kekurangan">Kekurangan</a></li>
                <li><a href="#kesimpulan">Kesimpulan</a></li>
            </ul>
        </div>
    </nav>

    <!-- Beranda Hero -->
    <section id="beranda">
        <div class="container hero-row">
            <div class="hero-teks">
                <h1>Teknologi <span>Fiber Optik</span> Penghubung Dunia Digital</h1>
                <p>Fiber Optik adalah teknologi transmisi data menggunakan cahaya melalui serat kaca halus, mampu mengirim informasi jarak jauh dengan kecepatan luar biasa untuk internet, telekomunikasi, dan jaringan masa depan dunia.</p>
                <a href="#tentang" class="tombol-utama">Pelajari Selengkapnya</a>
            </div>
            <img src="https://IMG_2002.JPEG"/photo-1558494945-851a41d35f8d?auto=format&fit=crop&w=500&q=80" alt="Fiber Optik Server" class="hero-gambar">
        </div>
    </section>

    <!-- Pengertian & Cara Kerja Fiber Optik -->
    <section id="tentang">
        <div class="container">
            <h2 class="judul-bagian">Apa Itu Fiber Optik?</h2>
            <div class="row-tentang">
                <img src="https://images.unsplash.com/photo-1558008229-3a0486b30903?auto=format&fit=crop&w=500&q=80" alt="Kabel Fiber Optik" class="gambar-tentang">
                <div class="teks-tentang">
                    <h3>Pengertian & Cara Kerja Fiber Optik</h3>
                    <p><strong>Fiber Optik (Serat Optik)</strong> adalah kabel komunikasi yang terbuat dari serat kaca atau plastik sangat halus, berfungsi sebagai media transmisi sinyal berupa cahaya untuk mengirim data dari satu tempat ke tempat lain.</p>
                    <p>Prinsip kerjanya menggunakan <strong>Refleksi Internal Total</strong>: cahaya yang masuk ke bagian inti (Core) akan terus dipantulkan berulang‑kali di dalam serat kaca tanpa keluar lapisan Cladding sehingga sinyal dapat menempuh jarak ribuan kilometer.</p>
                    <p>Teknologi ini menjadi tulang punggung komunikasi dunia untuk kabel bawah laut antar‑benua, internet rumah, kantor, pusat data, CCTV serta jaringan sekolah.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Kelebihan Fiber Optik -->
    <section id="kelebihan">
        <div class="container">
            <h2 class="judul-bagian">Kelebihan Utama Fiber Optik</h2>
            <div class="grid-4">
                <div class="card">
                    <div class="ikon-card">⚡</div>
                    <h4>Kecepatan Sangat Tinggi</h4>
                    <p>Mencapai puluhan hingga ratusan Gbps</p>
                </div>
                <div class="card">
                    <div class="ikon-card">🛡️</div>
                    <h4>Kebal Gangguan Elektromagnetik</h4>
                    <p>Tidak terganggu kabel listrik di sekitarnya</p>
                </div>
                <div class="card">
                    <div class="ikon-card">📏</div>
                    <h4>Jangkauan Sangat Jauh</h4>
                    <p>Sinyal tetap stabil jarak ribuan km</p>
                </div>
                <div class="card">
                    <div class="ikon-card">🔐</div>
                    <h4>Keamanan Data Tinggi</h4>
                    <p>Sulit disadap dibanding kabel tembaga</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Jenis Fiber Optik -->
    <section id="jenis">
        <div class="container">
            <h2 class="judul-bagian">Jenis‑Jenis Fiber Optik</h2>
            <div class="grid-2">
                <div class="card-2">
                    <h3>Single‑Mode Fiber (SMF)</h3>
                    <p>Inti serat sangat kecil (~9 µm), cahaya merambat lurus, untuk jarak jauh antar‑kota / kabel bawah laut sampai ratusan kilometer.</p>
                </div>
                <div class="card-2">
                    <h3>Multi‑Mode Fiber (MMF)</h3>
                    <p>Inti serat lebih besar (~50‑62,5 µm), cahaya merambat banyak jalur sekaligus, cocok untuk jaringan gedung, kampus, jarak pendek maksimal 2 km.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Komponen Utama -->
    <section id="komponen">
        <div class="container">
            <h2 class="judul-bagian">Komponen Utama Fiber Optik</h2>
            <div class="grid-2">
                <div class="card-2">
                    <h3>Bagian‑Bagian Kabel</h3>
                    <p>✅ Core (Inti)<br>✅ Cladding<br>✅ Coating Buffer<br>✅ Strength Member (Kevlar)<br>✅ Outer Jacket</p>
                </div>
                <div class="card-2">
                    <h3>Perangkat Pendukung</h3>
                    <p>✅ Fusion Splicer<br>✅ OTDR (Pengukur Kerusakan)<br>✅ ODB Kotak Terminal<br>✅ Patchcord & Pigtail</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Kekurangan Fiber Optik (Bagian Baru) -->
    <section id="kekurangan">
        <div class="container">
            <h2 class="judul-bagian">Kekurangan Fiber Optik</h2>
            <div class="grid-2">
                <div class="card-2">
                    <h3>Biaya Pemasangan Mahal</h3>
                    <p>Harga kabel serta alat penyambung fusion splicer relatif mahal dibandingkan kabel tembaga biasa.</p>
                </div>
                <div class="card-2">
                    <h3>Mudah Patah Jika Ditekuk Terlalu Kuat</h3>
                    <p>Inti serat terbuat dari kaca sehingga harus dipasang hati‑hati agar tidak bengkok terlalu tajam.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Kesimpulan Penutup (Bagian Baru) -->
    <section id="kesimpulan">
        <div class="container">
            <h2 class="judul-bagian">Kesimpulan & Penutup

