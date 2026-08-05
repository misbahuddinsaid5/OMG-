# my_first_profile
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Profesional | Misbahuddin Said</title>
    <!-- Menambahkan Font Google 'Poppins' agar lebih Estetik -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navbar Minimalis -->
    <nav>
        <div class="logo">M<span>.Said</span></div>
        <div class="right-nav">
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">Tentang</a></li>
                <li><a href="#projects">Proyek</a></li>
            </ul>
            <button id="theme-toggle" class="theme-btn">
                <span class="icon">🌙</span>
            </button>
        </div>
    </nav>

    <!-- Hero Section (Tampilan Utama) -->
    <header id="home" class="hero">
        <div class="hero-content">
            <h1 class="fade-in-down">Halo, Saya <span class="highlight">Misbahuddin Said</span></h1>
            <p class="fade-in">Mahasiswa kreatif di Universitas Muhammadiyah Malang yang berfokus pada Solusi Digital modern.</p>
            <div class="action-btns fade-in-up">
                <a href="#projects" class="btn btn-primary">Lihat Karya</a>
                <a href="#about" class="btn btn-secondary">Tentang Saya</a>
            </div>
        </div>
    </header>

    <!-- Tentang Saya (About) -->
    <section id="about" class="about">
        <div class="section-container">
            <h2 class="section-title">Tentang Saya</h2>
            <div class="about-content">
                <p>Saya adalah seorang mahasiswa Universitas Muhammadiyah Malang yang bersemangat dalam dunia teknologi. Saya memiliki minat mendalam pada pengembangan web dan desain UI/UX, dengan tujuan menciptakan pengalaman digital yang tidak hanya fungsional tetapi juga estetis dan mudah digunakan.</p>
            </div>
        </div>
    </section>

    <!-- Proyek (Projects) -->
    <section id="projects" class="projects">
        <div class="section-container">
            <h2 class="section-title">Proyek Saya</h2>
            <div class="project-grid">
                <!-- Kartu Proyek 1 -->
                <div class="project-card">
                    <div class="card-image placeholder-1"></div>
                    <div class="card-body">
                        <h3>Desain UI Modern</h3>
                        <p>Tugas kuliah merancang antarmuka aplikasi mobile yang responsif dan user-friendly.</p>
                        <a href="#" class="card-link">Detail Proyek →</a>
                    </div>
                </div>
                <!-- Kartu Proyek 2 -->
                <div class="project-card">
                    <div class="card-image placeholder-2"></div>
                    <div class="card-body">
                        <h3>Pengembangan Web</h3>
                        <p>Membangun landing page estetik menggunakan HTML, CSS, dan JavaScript dasar.</p>
                        <a href="#" class="card-link">Detail Proyek →</a>
                    </div>
                </div>
                <!-- Kartu Proyek 3 -->
                <div class="project-card">
                    <div class="card-image placeholder-3"></div>
                    <div class="card-body">
                        <h3>Portofolio Kuliah</h3>
                        <p>Kumpulan karya dan tugas terbaik saya selama studi di UMM.</p>
                        <a href="#" class="card-link">Detail Proyek →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Misbahuddin Said. Proudly a UMM Student.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>


/* --- CSS Reset & Variabel Estetik --- */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif; /* Menggunakan font Poppins */
    scroll-behavior: smooth;
}

:root {
    /* Skema Warna Terang (Light Mode) */
    --bg-body: #ffffff;
    --bg-nav: rgba(255, 255, 255, 0.95);
    --text-main: #333333;
    --text-muted: #666666;
    --accent-color: #6c5ce7; /* Warna aksen ungu modern */
    --accent-hover: #5a4bcf;
    --card-bg: #ffffff;
    --card-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
    --border-color: #eeeeee;
    
    /* Transisi Halus */
    --transition-fast: 0.2s ease;
    --transition-slow: 0.4s ease;
}

/* --- Variabel Mode Gelap (Dark Mode) --- */
.dark-theme {
    --bg-body: #121212;
    --bg-nav: rgba(18, 18, 18, 0.98);
    --text-main: #f5f5f5;
    --text-muted: #b0b0b0;
    --accent-color: #a29bfe; /* Warna ungu lebih terang untuk dark mode */
    --accent-hover: #beb7ff;
    --card-bg: #1e1e1e;
    --card-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    --border-color: #333333;
}

body {
    background-color: var(--bg-body);
    color: var(--text-main);
    transition: background-color var(--transition-slow), color var(--transition-slow);
    line-height: 1.6;
}

/* --- Navigasi Minimalis & Transparan --- */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 10%;
    background-color: var(--bg-nav);
    backdrop-filter: blur(10px); /* Efek blur kaca */
    position: sticky;
    top: 0;
    z-index: 1000;
    border-bottom: 1px solid var(--border-color);
}

nav .logo {
    font-size: 24px;
    font-weight: 700;
    letter-spacing: -1px;
}

nav .logo span {
    color: var(--accent-color);
}

.right-nav {
    display: flex;
    align-items: center;
    gap: 20px;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    text-decoration: none;
    color: var(--text-main);
    font-weight: 400;
    font-size: 15px;
    transition: color var(--transition-fast);
}

.nav-links a:hover {
    color: var(--accent-color);
}

/* Tombol Mode Gelap Estetik */
.theme-btn {
    background: none;
    border: 1px solid var(--border-color);
    cursor: pointer;
    padding: 8px;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: background var(--transition-fast);
}

.theme-btn:hover {
    background-color: var(--border-color);
}

/* --- Hero Section yang Elegan --- */
.hero {
    height: 90vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
    /* Gradasi latar belakang halus */
    background: radial-gradient(circle at center, var(--border-color) 0%, var(--bg-body) 70%);
}

.hero h1 {
    font-size: 56px;
    font-weight: 800;
    letter-spacing: -2px;
    margin-bottom: 15px;
    line-height: 1.1;
}

.highlight {
    color: var(--accent-color);
}

.hero p {
    font-size: 18px;
    color: var(--text-muted);
    max-width: 600px;
    margin: 0 auto 35px auto;
    font-weight: 300;
}

/* Tombol-tombol Aksi */
.action-btns {
    display: flex;
    justify-content: center;
    gap: 15px;
}

.btn {
    display: inline-block;
    padding: 12px 30px;
    text-decoration: none;
    border-radius: 50px; /* Tombol membulat */
    font-weight: 600;
    font-size: 15px;
    transition: all var(--transition-fast);
}

.btn-primary {
    background-color: var(--accent-color);
    color: white;
}

.btn-primary:hover {
    background-color: var(--accent-hover);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(108, 92, 231, 0.3);
}

.btn-secondary {
    background-color: transparent;
    color: var(--text-main);
    border: 1px solid var(--border-color);
}

.btn-secondary:hover {
    background-color: var(--border-color);
}

/* --- Pengaturan Section Umum --- */
section {
    padding: 100px 0;
}

.section-container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
}

.section-title {
    text-align: center;
    font-size: 36px;
    font-weight: 700;
    margin-bottom: 50px;
    letter-spacing: -1px;
}

.section-title::after {
    content: '';
    display: block;
    width: 60px;
    height: 4px;
    background-color: var(--accent-color);
    margin: 10px auto 0 auto;
    border-radius: 2px;
}

/* --- About Section --- */
.about-content {
    max-width: 800px;
    margin: 0 auto;
    text-align: center;
    font-size: 17px;
    color: var(--text-muted);
    font-weight: 300;
}

/* --- Projects Grid & Cards Modern --- */
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 30px;
}

.project-card {
    background-color: var(--card-bg);
    border-radius: 16px; /* Sudut membulat modern */
    overflow: hidden;
    box-shadow: var(--card-shadow);
    transition: transform var(--transition-fast), box-shadow var(--transition-fast);
    border: 1px solid var(--border-color);
}

.project-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
}

/* Placeholder Gambar Proyek */
.card-image {
    height: 200px;
    width: 100%;
}

/* Gradasi warna estetik untuk gambar placeholder */
.placeholder-1 { background: linear-gradient(135deg, #89f7fe 0%, #66a6ff 100%); }
.placeholder-2 { background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); }
.placeholder-3 { background: linear-gradient(135deg, #5ee7df 0%, #b490ca 100%); }

.card-body {
    padding: 25px;
}

.card-body h3 {
    font-size: 20px;
    font-weight: 600;
    margin-bottom: 10px;
}

.card-body p {
    font-size: 14px;
    color: var(--text-muted);
    margin-bottom: 20px;
    font-weight: 300;
}

.card-link {
    text-decoration: none;
    color: var(--accent-color);
    font-weight: 600;
    font-size: 14px;
    transition: color var(--transition-fast);
}

.card-link:hover {
    color: var(--accent-hover);
}

/* --- Footer --- */
footer {
    text-align: center;
    padding: 40px;
    border-top: 1px solid var(--border-color);
    font-size: 14px;
    color: var(--text-muted);
    font-weight: 300;
}

/* --- Animasi Dasar (Fade In) --- */
@keyframes fadeInDown {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.fade-in-down { animation: fadeInDown 0.8s ease forwards; }
.fade-in { animation: fadeIn 1s ease 0.4s forwards; opacity: 0; }
.fade-in-up { animation: fadeInUp 0.8s ease 0.8s forwards; opacity: 0; }

/* --- Responsivitas untuk Mobile --- */
@media (max-width: 768px) {
    .hero h1 { font-size: 40px; }
    .hero p { font-size: 16px; }
    
    .nav-links { display: none; } /* Sembunyikan link nav di mobile untuk kesederhanaan */
    nav { padding: 15px 5%; }
}


const themeToggle = document.getElementById('theme-toggle');
const body = document.body;
const iconSpan = themeToggle.querySelector('.icon');

// Cek preferensi tema pengguna yang tersimpan di browser
const currentTheme = localStorage.getItem('theme');
if (currentTheme) {
    body.classList.add(currentTheme);
    updateIcon();
}

themeToggle.addEventListener('click', () => {
    // Toggle class dark-theme
    body.classList.toggle('dark-theme');
    
    // Simpan preferensi tema
    let theme = 'light';
    if (body.classList.contains('dark-theme')) {
        theme = 'dark';
    }
    localStorage.setItem('theme', theme + '-theme');
    
    // Update ikon tombol
    updateIcon();
});

// Fungsi untuk mengupdate ikon (Bulan/Matahari)
function updateIcon() {
    if (body.classList.contains('dark-theme')) {
        iconSpan.textContent = '☀️'; // Ikon Matahari untuk Mode Terang
    } else {
        iconSpan.textContent = '🌙'; // Ikon Bulan untuk Mode Gelap
    }
}