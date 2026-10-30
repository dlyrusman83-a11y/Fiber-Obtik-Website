
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fiber Optik Indonesia | Teknologi Masa Depan</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --biru-tua: #0c4a6e;
            --biru: #0284c7;
            --biru-muda: #38bdf8;
            --cyan: #06b6d4;
            --gelap: #1e293b;
            --terang: #f8fafc;
            --abu: #64748b;
            --putih: #ffffff;
        }

        body {
            line-height: 1.7;
            color: var(--gelap);
            background-color: #f0f9ff;
        }

        /* Navigasi */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255,255,255,0.95);
            box-shadow: 0 2px 12px rgba(0,0,0,0.08);
            z-index: 999;
        }

        .nav-wrap {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.4rem;
            font-weight: 700;
            color: var(--biru);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .nav-menu {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-menu a {
            text-decoration: none;
            color: var(--gelap);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-menu a:hover {
            color: var(--biru);
        }

        .menu-btn {
            display: none;
            font-size: 1.8rem;
            cursor: pointer;
        }

        /* Bagian Hero */
        .hero {
            margin-top: 70px;
            background: linear-gradient(135deg, var(--biru-tua), var(--biru));
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 3rem 2rem;
            color: var(--putih);
        }

        .hero-grid {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .hero h1 {
            font-size: 2.8rem;
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }

        .hero p {
            font-size: 1.1rem;
            margin-bottom: 2rem;
            opacity: 0.92;
        }

        .btn {
            display: inline-block;
            padding: 0.85rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
        }

        .btn-utama {
            background: var(--putih);
            color: var(--biru);
            margin-right: 0.8rem;
        }

        .btn-utama:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .btn-kedua {
            border: 2px solid white;
            color: white;
            background: transparent;
        }

        .btn-kedua:hover {
            background: white;
            color: var(--biru);
        }

        .hero-gambar {
            background: url('https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=600') center/cover no-repeat;
            height: 400px;
            border-radius: 16px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
        }

        /* Bagian Umum */
        section {
            padding: 4.5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .judul-bagian {
            text-align: center;
            font-size: 2rem;
            color: var(--biru-tua);
            margin-bottom: 3rem;
            position: relative;
        }

        .judul-bagian::after {
            content: '';
            position: absolute;
            width: 70px;
            height: 4px;
            background: var(--cyan);
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }

        /* Apa itu Fiber Optik */
        .penjelasan-wrap {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .gambar-ilustrasi {
            background: url('https://images.unsplash.com/photo-1544197150-b99a580bb7a8?w=600') center/cover no-repeat;
            height: 350px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
        }

        .teks h3 {
            font-size: 1.4rem;
            color: var(--biru);
            margin-bottom: 1rem;
        }

        .teks p {
            margin-bottom: 1rem;
            color: var(--abu);
        }

        /* Kelebihan */
        #kelebihan {
            background: var(--terang);
        }

        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 1.8rem;
        }

        .kartu {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.04);
            border-left: 4px solid var(--biru);
            transition: transform 0.3s;
        }

        .kartu:hover {
            transform: translateY(-6px);
        }

        .kartu .ikon {
            font-size: 2.2rem;
            margin-bottom: 1rem;
        }

        .kartu h4 {
            font-size: 1.15rem;
            color: var(--biru-tua);
            margin-bottom: 0.7rem;
        }

        .kartu p {
            color: var(--abu);
            font-size: 0.95rem;
        }

        /* Jenis Fiber */
        .jenis-wrap {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .jenis-kartu {
            padding: 2rem;
            border-radius: 12px;
            background: linear-gradient(145deg, #ffffff, #e0f2fe);
            border: 1px solid #bae6fd;
        }

        .jenis-kartu h4 {
            font-size: 1.3rem;
            color: var(--biru-tua);
            margin-bottom: 1rem;
        }

        .jenis-kartu span {
            display: inline-block;
            background: var(--biru-muda);
            color: white;
            padding: 0.25rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
            margin-bottom: 1rem;
        }

        /* Komponen */
        #komponen {
            background-color: var(--terang);
        }

        .daftar-komponen {
            background: white;
            border-radius: 12px;
            padding: 2.5rem;
            box-shadow: 0 4px 14px rgba(0,0,0,0.04);
        }

        .daftar-komponen ul {
            list-style: none;
            margin-top: 1rem;
        }

        .daftar-komponen li {
            padding: 0.8rem 0;
            border-bottom: 1px solid #e2e8f0;
        }

        .daftar-komponen li strong {
            color: var(--biru);
        }

        /* Kontak */
        #kontak {
            background: var(--biru-tua);
            color: white;
            border-radius: 16px;
            margin: 2rem;
            max-width: 1160px;
        }

        #kontak .judul-bagian {
            color: white;
        }

        .kontak-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        .info-kontak p {
            margin-bottom: 1rem;
            opacity: 0.9;
        }

        .form-kontak input,
        .form-kontak textarea {
            width: 100%;
            padding: 0.9rem;
            margin-bottom: 1rem;
            border-radius: 8px;
            border: none;
            font-size: 1rem;
        }

        .form-kontak button {
            background: var(--cyan);
            color: white;
            border: none;
            padding: 0.9rem 2rem;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }

        .form-kontak button:hover {
            background: #0891b2;
        }

        /* Footer */
        footer {
            background: var(--gelap);
            color: white;
            text-align: center;
            padding: 2rem;
            font-size: 0.95rem;
        }

        /* Responsif */
        @media (max-width: 768px) {
            .menu-btn {
                display: block;
            }

            .nav-menu {
                position: absolute;
                top: 65px;
                left: 0;
                width: 100%;
                background: white;
                flex-direction: column;
                padding: 1rem 2rem;
                gap: 1rem;
                display: none;
                box-shadow: 0 8px 10px rgba(0,0,0,0.05);
            }

            .nav-menu.tampil {
                display: flex;
            }

            .hero-grid, .penjelasan-wrap, .kontak-grid {
                grid-template-columns: 1fr;
            }

            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Navigasi -->
    <nav>
        <div class="nav-wrap">
            <div class="logo">🔷 FiberOptik</div>
            <div class="menu-btn" id="menuBtn">☰</div>
            <ul class="nav-menu" id="navMenu">
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Apa Itu?</a></li>
                <li><a href="#kelebihan">Kelebihan</a></li>
                <li><a href="#jenis">Jenis</a></li>
                <li><a href="#komponen">Komponen</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </div>
    </nav>

    <!-- Beranda/Hero -->
    <section class="hero" id="beranda">
        <div class="hero-grid">
            <div>
                <h1>Internet Super Cepat Menggunakan Teknologi <span style="color:#a5f3fc">Fiber Optik</span></h1>
                <p>Transmisi data tercepat dan paling stabil di dunia. Menggunakan cahaya untuk mengirim informasi, menghadirkan koneksi tanpa batas untuk rumah, bisnis, dan kota pintar.</p>
                <a href="#tentang" class="btn btn-utama">Pelajari Lebih Lanjut</a>
                <a href="#kontak" class="btn btn-kedua">Hubungi Kami</a>
            </div>
            <div class="hero-gambar"></div>
        </div>
    </section>

    <!-- Apa Itu Fiber Optik -->
    <section id="tentang">
        <h2 class="judul-bagian">Apa Itu Fiber Optik?</h2>
        <div class="penjelasan-wrap">
            <div class="gambar-ilustrasi"></div>
            <div class="teks">
                <h3>Kabel Serat Optik — Teknologi Masa Depan</h3>
                <p><strong>Fiber optik</strong> atau serat optik adalah kabel yang terbuat dari kaca atau plastik yang sangat halus, berfungsi sebagai media transmisi sinyal cahaya dari satu tempat ke tempat lain.</p>
                <p>Cahaya yang dijalarkan di dalam inti serat memantul berulang kali sepanjang kabel, memungkinkan data dikirim dengan kecepatan sangat tinggi hingga <strong>ratusan Gigabit per detik</strong>, jauh lebih cepat daripada kabel tembaga konvensional.</p>
                <p>Teknologi ini menjadi tulang punggung internet global, menghubungkan benua-benua di bawah lautan dan membawa internet stabil ke rumah-rumah di seluruh dunia.</p>
            </div>
        </div>
    </section>

    <!-- Kelebihan -->
    <section id="kelebihan">
        <h2 class="judul-bagian">Kelebihan Fiber Optik</h2>
        <div class="grid-3">
            <div class="kartu">
                <div class="ikon">⚡</div>
                <h4>Kecepatan Sangat Tinggi</h4>
                <p>Mampu mentransfer data hingga 100 Gbps bahkan lebih, ratusan kali lebih cepat dari kabel tembaga biasa.</p>
            </div>
            <div class="kartu">
                <div class="ikon">🛡️</div>
                <h4>Aman & Bebas Gangguan</h4>
                <p>Tidak terpengaruh gangguan gelombang elektromagnetik dan sulit disadap, sehingga data lebih aman.</p>
            </div>
            <div class="kartu">
                <div class="ikon">📏</div>
                <h4>Jarak Jangkauan Jauh</h4>
                <p>Sinyal dapat menempuh jarak puluhan kilometer tanpa perlu diperkuat ulang.</p>
            </div>
            <div class="kartu">
                <div class="ikon">💪</div>
                <h4>Kapasitas Besar</h4>
                <p>Satu kabel tipis dapat menampung ribuan saluran telepon dan ribuan siaran TV sekaligus.</p>
            </div>
            <div class="kartu">
                <div class="ikon">🌡️</div>
                <h4>Tahan Lingkungan</h4>
                <p>Lebih tahan terhadap perubahan suhu dan kelembapan dibandingkan kabel tembaga.</p>
            </div>
            <div class="kartu">
                <div class="ikon">🌍</div>
                <h4>Hemat Energi</h4>
                <p>Sinyal cahaya membutuhkan lebih sedikit daya listrik dibandingkan sinyal listrik konvensional.</p>
            </div>
        </div>
    </section>

    <!-- Jenis Fiber Optik -->
    <section id="jenis">
        <h2 class="judul-bagian">Jenis-Jenis Fiber Optik</h2>
        <div class="jenis-wrap">
            <div class="jenis-kartu">
                <h4>🔹 Single-Mode Fiber (SMF)</h4>
                <span>Inti Kecil & Jarak Jauh</span>
                <p>Memiliki inti sangat kecil (~9 mikrometer), membiarkan cahaya merambat lurus ke satu arah. Digunakan untuk sambungan jarak jauh antar kota maupun antar negara, serta kabel bawah laut.</p>
                <p><strong>Jarak:</strong> 2 km – 100+ km tanpa penguat sinyal.</p>
            </div>
            <div class="jenis-kartu">
                <h4>🔸 Multi-Mode Fiber (MMF)</h4>
                <span>Inti Lebih Besar & Jarak Pendek</span>
                <p>Inti lebih besar (~50/62,5 mikrometer), cahaya merambat dalam banyak jalur sekaligus. Lebih murah dan mudah dipasang, cocok untuk jaringan dalam gedung, perkantoran, atau pusat data.</p>
                <p><strong>Jarak:</strong> Maksimal sekitar 500 meter – 2 km.</p>
            </div>
        </div>
    </section>

    <!-- Komponen -->
    <section id="komponen">
        <h2 class="judul-bagian">Komponen Utama Fiber Optik</h2>
        <div class="daftar-komponen">
            <ul>
                <li><strong>🔹 Inti (
                
