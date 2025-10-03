<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Situs Web Responsif</title>

    <!-- Favicon -->
    <link rel="icon" href="https://via.placeholder.com/32x32.png?text=🌐" type="image/png">

    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">

    <!-- Meta SEO -->
    <meta name="description" content="Contoh situs web responsif menggunakan HTML dan CSS. Cocok untuk pemula belajar desain web.">

    <style>
        /* Reset dan Font */
        * {
            box-sizing: border-box;
        }
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #e9ecef;
            color: #333;
        }

        /* Navbar */
        nav {
            background-color: #1e7e34;
            color: white;
            padding: 15px 20px;
        }

        nav .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1100px;
            margin: auto;
        }

        nav h2 {
            margin: 0;
            font-size: 1.2em;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            gap: 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
        }

        /* Header */
        header {
            background-color: #28a745;
            color: white;
            padding: 30px;
            text-align: center;
            margin-bottom: 20px;
        }

        .container {
            width: 90%;
            max-width: 1100px;
            margin: auto;
            overflow: hidden;
            padding: 0 10px;
        }

        /* Tata Letak 2 Kolom */
        .main-content {
            display: flex;
            gap: 20px;
        }

        .main-article {
            flex: 3;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .sidebar {
            flex: 1;
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            max-height: fit-content;
        }

        .featured-image {
            width: 100%;
            height: auto;
            border-radius: 6px;
            margin-bottom: 15px;
        }

        footer {
            text-align: center;
            padding: 15px;
            background-color: #343a40;
            color: white;
            margin-top: 30px;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            .main-content {
                flex-direction: column;
            }
            .main-article, .sidebar {
                flex: none;
                width: 100%;
            }
            .sidebar {
                margin-top: 20px;
            }
            header h1 {
                font-size: 1.5em;
            }

            nav ul {
                flex-direction: column;
                gap: 10px;
            }
        }
    </style>
</head>
<body>

    <!-- Navigasi -->
    <nav role="navigation" aria-label="Navigasi utama">
        <div class="nav-container">
            <h2>LogoWeb</h2>
            <ul>
                <li><a href="#">Beranda</a></li>
                <li><a href="#">Tentang</a></li>
                <li><a href="#">Kontak</a></li>
            </ul>
        </div>
    </nav>

    <!-- Header -->
    <header>
        <h1>Web Responsif Siap Ponsel</h1>
        <p>Lihat hasilnya di desktop, lalu coba ubah ukuran browser Anda!</p>
    </header>

    <div class="container">
        <div class="main-content">
            
            <div class="main-article">
                <h2>Pentingnya Desain Responsif</h2>
                <p>
                    Ini adalah konten utama. Dengan <strong>Media Query</strong> di CSS, kita memastikan bahwa pengalaman 
                    pengguna tetap baik di semua ukuran layar.
                </p>

                <img src="https://via.placeholder.com/600x300?text=Situs+Responsif" alt="Gambar Contoh Desain Web" class="featured-image">

                <p>
                    Cobalah <strong>memperkecil jendela browser</strong> Anda. Begitu lebar jendela mencapai 768px atau kurang, 
                    sidebar akan pindah ke bawah artikel utama.
                </p>

                <p>
                    Ini dicapai hanya dengan beberapa baris kode CSS di dalam <code>@media (max-width: 768px)</code>.
                </p>
            </div>

            <div class="sidebar">
                <h3>Fitur di Ponsel</h3>
                <p>
                    Bagian ini akan berada di samping pada desktop, namun akan berpindah ke bawah konten utama ketika dilihat di ponsel.
                </p>
                <h4>Tautan Cepat</h4>
                <ul>
                    <li><a href="#">Fitur Baru</a></li>
                    <li><a href="#">Blog Terbaru</a></li>
                    <li><a href="#">Gabung Newsletter</a></li>
                </ul>
            </div>

        </div>
    </div>

    <footer>
        <p>Situs Web Sederhana dan Responsif | &copy; 2025</p>
    </footer>

</body>
</html>
