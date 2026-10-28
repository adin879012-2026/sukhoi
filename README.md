<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Website Personal | Nama Anda</title>

    <meta name="description" content="Website personal untuk memperkenalkan diri, keahlian, dan portofolio saya.">

    <style>
        /* RESET */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f8fafc;
            color: #1e293b;
            line-height: 1.7;
        }

        /* NAVBAR */
        header {
            background: #ffffff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav {
            max-width: 1100px;
            margin: auto;
            padding: 15px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
            color: #2563eb;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav a {
            text-decoration: none;
            color: #334155;
            font-size: 14px;
            transition: 0.3s;
        }

        nav a:hover {
            color: #2563eb;
        }

        /* HERO */
        .hero {
            min-height: 85vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 70px 20px;
            background: linear-gradient(135deg, #eff6ff, #ffffff);
        }

        .hero-content {
            max-width: 750px;
        }

        .profile-photo {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid #ffffff;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.12);
            margin-bottom: 25px;
            background: #dbeafe;
        }

        .hero h1 {
            font-size: clamp(30px, 5vw, 48px);
            margin-bottom: 10px;
            color: #0f172a;
        }

        .hero h1 span {
            color: #2563eb;
        }

        .hero p {
            color: #64748b;
            font-size: 17px;
            margin-bottom: 25px;
        }

        .button {
            display: inline-block;
            background: #2563eb;
            color: #ffffff;
            padding: 12px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
            margin: 5px;
        }

        .button:hover {
            background: #1d4ed8;
            transform: translateY(-2px);
        }

        .button-outline {
            background: transparent;
            color: #2563eb;
            border: 1px solid #2563eb;
        }

        .button-outline:hover {
            color: #ffffff;
        }

        /* GENERAL SECTION */
        section {
            padding: 75px 20px;
        }

        .container {
            max-width: 1000px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            font-size: 30px;
            margin-bottom: 15px;
            color: #0f172a;
        }

        .section-description {
            text-align: center;
            color: #64748b;
            max-width: 650px;
            margin: 0 auto 40px;
        }

        /* ABOUT */
        .about-card {
            background: #ffffff;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.04);
        }

        .about-card p {
            color: #475569;
            margin-bottom: 15px;
        }

        /* SKILLS */
        #keahlian {
            background: #ffffff;
        }

        .skills {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .skill-card {
            background: #f8fafc;
            padding: 25px 20px;
            border-radius: 12px;
            text-align: center;
            border: 1px solid #e2e8f0;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-5px);
            border-color: #2563eb;
        }

        .skill-card .icon {
            font-size: 35px;
            margin-bottom: 10px;
        }

        .skill-card h3 {
            margin-bottom: 8px;
            color: #1e293b;
        }

        .skill-card p {
            color: #64748b;
            font-size: 14px;
        }

        /* CONTACT */
        .contact-card {
            text-align: center;
            background: #ffffff;
            border-radius: 15px;
            padding: 40px 25px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.04);
        }

        .contact-card p {
            color: #64748b;
            margin-bottom: 20px;
        }

        /* FOOTER */
        footer {
            background: #0f172a;
            color: #cbd5e1;
            text-align: center;
            padding: 25px 15px;
            font-size: 14px;
        }

        footer a {
            color: #93c5fd;
            text-decoration: none;
        }

        /* RESPONSIVE */
        @media (max-width: 650px) {
            nav {
                flex-direction: column;
                gap: 10px;
            }

            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }

            nav a {
                font-size: 13px;
            }

            .skills {
                grid-template-columns: 1fr;
            }

            .hero {
                min-height: 75vh;
            }

            section {
                padding: 55px 18px;
            }
        }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <header>
        <nav>
            <div class="logo">PersonalWeb.</div>

            <ul>
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Tentang</a></li>
                <li><a href="#keahlian">Keahlian</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <!-- BERANDA -->
    <section class="hero" id="beranda">
        <div class="hero-content">

            <!-- Ganti foto.jpg dengan foto Anda -->
            <img
                src="foto.jpg"
                alt="Foto profil saya"
                class="profile-photo"
            >

            <h1>Halo, Saya <span>Nama Anda</span></h1>

            <p>
                Selamat datang di website personal saya.
                Saya tertarik pada teknologi, kreativitas,
                pengembangan diri, dan hal-hal baru.
            </p>

            <a href="#tentang" class="button">
                Tentang Saya
            </a>

            <a
                href="https://wa.me/6281234567890"
                class="button button-outline"
                target="_blank"
                rel="noopener noreferrer"
            >
                Hubungi Saya
            </a>

        </div>
    </section>

    <!-- TENTANG SAYA -->
    <section id="tentang">
        <div class="container">

            <h2 class="section-title">Tentang Saya</h2>

            <p class="section-description">
                Mengenal saya lebih dekat.
            </p>

            <div class="about-card">
                <p>
                    Perkenalkan, nama saya <strong>Nama Anda</strong>.
                    Saya adalah seseorang yang senang belajar,
                    mengembangkan kemampuan, dan mencoba hal-hal baru.
                </p>

                <p>
                    Saya memiliki ketertarikan dalam bidang teknologi,
                    administrasi, pengembangan website, dan kreativitas.
                    Saya percaya bahwa proses belajar yang konsisten
                    merupakan kunci untuk terus berkembang.
                </p>

                <p>
                    Website ini dibuat sebagai tempat untuk memperkenalkan
                    diri, membagikan informasi, dan membangun koneksi
                    dengan orang lain.
                </p>
            </div>

        </div>
    </section>

    <!-- KEAHLIAN -->
    <section id="keahlian">
        <div class="container">

            <h2 class="section-title">Keahlian Saya</h2>

            <p class="section-description">
                Beberapa bidang yang saya minati dan kembangkan.
            </p>

            <div class="skills">

                <div class="skill-card">
                    <div class="icon">💻</div>
                    <h3>Teknologi</h3>
                    <p>
                        Mengenal teknologi digital dan
                        pengembangan website.
                    </p>
                </div>

                <div class="skill-card">
                    <div class="icon">📊</div>
                    <h3>Administrasi</h3>
                    <p>
                        Pengelolaan dokumen, data, dan
                        pekerjaan administratif.
                    </p>
                </div>

                <div class="skill-card">
                    <div class="icon">🚀</div>
                    <h3>Pengembangan Diri</h3>
                    <p>
                        Terus belajar, meningkatkan kemampuan,
                        dan mengembangkan ide kreatif.
                    </p>
                </div>

            </div>

        </div>
    </section>

    <!-- KONTAK -->
    <section id="kontak">
        <div class="container">

            <h2 class="section-title">Hubungi Saya</h2>

            <p class="section-description">
                Mari terhubung dan berbagi ide.
            </p>

            <div class="contact-card">

                <p>
                    Anda dapat menghubungi saya melalui WhatsApp
                    atau mengunjungi media sosial saya.
                </p>

                <a
                    href="https://wa.me/6281234567890"
                    class="button"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    WhatsApp
                </a>

                <a
                    href="https://www.instagram.com/usernameanda/"
                    class="button button-outline"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    Instagram
                </a>

                <a
                    href="https://github.com/usernameanda"
                    class="button button-outline"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    GitHub
                </a>

            </div>

        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>
            &copy; <span id="tahun"></span> Nama Anda.
            Dibuat dengan HTML dan CSS.
        </p>
    </footer>

    <script>
        // Menampilkan tahun secara otomatis
        document.getElementById("tahun").textContent =
            new Date().getFullYear();
    </script>

</body>
</html>
