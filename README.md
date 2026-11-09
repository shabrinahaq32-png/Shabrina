<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shabrina Namsikul Haq | Futuristic Profile</title>
    <style>
        /* Base Reset & Variables */
        :root {
            --bg-dark: #0a0a12;
            --bg-card: rgba(20, 20, 35, 0.7);
            --neon-blue: #00f0ff;
            --neon-purple: #bd00ff;
            --text-main: #e2e8f0;
            --text-muted: #94a3b8;
            --font-cyber: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            font-family: var(--font-cyber);
            overflow-x: hidden;
            line-height: 1.6;
            background-image: 
                radial-gradient(circle at 20% 30%, rgba(0, 240, 255, 0.05) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(189, 0, 255, 0.05) 0%, transparent 40%);
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: var(--bg-dark);
        }
        ::-webkit-scrollbar-thumb {
            background: rgba(0, 240, 255, 0.3);
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: var(--neon-blue);
        }

        /* Header & Navigation */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            padding: 1.5rem 10%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(10, 10, 18, 0.8);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(0, 240, 255, 0.1);
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 2px;
            background: linear-gradient(45deg, var(--neon-blue), var(--neon-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 10px rgba(0, 240, 255, 0.2);
        }

        nav a {
            color: var(--text-main);
            text-decoration: none;
            margin-left: 2rem;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: 0.3s ease;
        }

        nav a:hover {
            color: var(--neon-blue);
            text-shadow: 0 0 8px var(--neon-blue);
        }

        /* Container Blueprint */
        section {
            padding: 8rem 10% 4rem 10%;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        /* Hero Section */
        #hero {
            position: relative;
        }

        .glitch-title {
            font-size: 4rem;
            font-weight: 900;
            line-height: 1.1;
            margin-bottom: 1rem;
            letter-spacing: -1px;
        }

        .glitch-title span {
            display: block;
            background: linear-gradient(to right, #fff, var(--text-muted));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .highlight {
            color: var(--neon-blue);
            text-shadow: 0 0 15px rgba(0, 240, 255, 0.4);
            -webkit-text-fill-color: initial !important;
        }

        .subtitle {
            font-size: 1.25rem;
            color: var(--text-muted);
            max-width: 600px;
            margin-bottom: 2.5rem;
        }

        .cta-btn {
            display: inline-block;
            padding: 0.8rem 2rem;
            border: 1px solid var(--neon-blue);
            background: transparent;
            color: var(--neon-blue);
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 2px;
            text-decoration: none;
            position: relative;
            overflow: hidden;
            transition: 0.3s ease;
            width: fit-content;
        }

        .cta-btn:hover {
            background: var(--neon-blue);
            color: var(--bg-dark);
            box-shadow: 0 0 25px rgba(0, 240, 255, 0.5);
        }

        /* Section Headings */
        .section-header {
            margin-bottom: 4rem;
        }

        .section-header h2 {
            font-size: 2rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            position: relative;
            display: inline-block;
        }

        .section-header h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 50px;
            height: 2px;
            background: var(--neon-purple);
            box-shadow: 0 0 8px var(--neon-purple);
        }

        /* Grid Layouts */
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 11fr));
            gap: 2.5rem;
        }

        /* Cards Design (Futuristic Cyberpunk Minimalist) */
        .cyber-card {
            background: var(--bg-card);
            border: 1px solid rgba(255, 255, 255, 0.05);
            padding: 2.5rem;
            position: relative;
            transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
            backdrop-filter: blur(8px);
        }

        .cyber-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--neon-blue);
            transition: 0.4s ease;
        }

        .cyber-card:hover {
            transform: translateY(-5px);
            border-color: rgba(0, 240, 255, 0.2);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }

        .cyber-card:hover::before {
            width: 100%;
        }

        /* Skills Layout */
        .skills-wrapper {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
        }

        .skill-tag {
            background: rgba(255, 255, 255, 0.02);
            border: 1px solid rgba(255, 255, 255, 0.08);
            padding: 1rem;
            text-align: center;
            font-weight: 500;
            letter-spacing: 1px;
            transition: 0.3s;
        }

        .skill-tag:hover {
            background: rgba(0, 240, 255, 0.03);
            border-color: var(--neon-blue);
            color: var(--neon-blue);
            text-shadow: 0 0 5px rgba(0, 240, 255, 0.5);
        }

        /* Project Styles */
        .project-title {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            color: #fff;
        }

        .project-desc {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 1.5rem;
        }

        .project-tech {
            font-size: 0.8rem;
            text-transform: uppercase;
            color: var(--neon-purple);
            letter-spacing: 1px;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 3rem;
            font-size: 0.85rem;
            color: var(--text-muted);
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            letter-spacing: 1px;
        }

        /* Responsive Settings */
        @media (max-width: 768px) {
            .glitch-title { font-size: 2.5rem; }
            header { padding: 1.5rem 5%; }
            section { padding: 6rem 5% 3rem 5%; }
            nav { display: none; } /* Simplified for mobile flow */
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <div class="logo">SNH // O1</div>
        <nav>
            <a href="#hero">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
        </nav>
    </header>

    <!-- Main Hero Interface -->
    <section id="hero">
        <h1 class="glitch-title">
            <span>SHABRINA NAMSIKUL HAQ</span>
            <span class="highlight">SOFTWARE ENGINEER</span>
        </h1>
        <p class="subtitle">
            Mahasiswi semester 1 di Politeknik Indonusa Surakarta. Berfokus pada arsitektur web modern dan pembuatan antarmuka digital interaktif berkinerja tinggi.
        </p>
        <a href="#projects" class="cta-btn">Lihat Proyek</a>
    </section>

    <!-- About / Background Section -->
    <section id="about">
        <div class="section-header">
            <h2>Latar Belakang</h2>
        </div>
        <div class="grid-container">
            <div class="cyber-card">
                <p>Memulai perjalanan akademis di bidang Rekayasa Perangkat Lunak (Software Engineering), saya mendedikasikan diri untuk memahami bagaimana baris kode dapat bertransformasi menjadi solusi platform yang elegan, solutif, dan berdampak nyata bagi pengguna.</p>
            </div>
            <div class="cyber-card">
                <p>Bagi saya, pemrograman bukan sekadar instruksi mesin, melainkan jembatan kreativitas manusia. Saya berfokus untuk menghasilkan produk web bersih, berstruktur rapi, dan memiliki estetika visual yang kuat.</p>
            </div>
        </div>
    </section>

    <!-- Skills Core Section -->
    <section id="skills">
        <div class="section-header">
            <h2>Kombinasi Teknologi</h2>
        </div>
        <div class="skills-wrapper">
            <div class="skill-tag">HTML5 Engine</div>
            <div class="skill-tag">CSS3 / Architecture</div>
            <div class="skill-tag">JavaScript ES6+</div>
            
