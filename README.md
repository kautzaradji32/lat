<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio- Adji Pramudya K | Desainer & Pengembang Web Profesional</title>
    <meta name="description" content="Portfolio profesional [Nama Anda] dengan showcase karya terbaik dalam desain web, pengembangan, dan kreativitas digital. SEO optimized portfolio.">
    <meta name="keywords" content="portfolio, desain web, pengembangan web, kreatif, UI/UX, SEO">
    <meta name="author" content="[Nama Anda]">
    <meta property="og:title" content="Portfolio Kreatif - [Nama Anda]">
    <meta property="og:description" content="Kumpulan karya terbaik [Nama Anda] dalam desain dan pengembangan web">
    
    <style>
        /* Reset & Base Styles */
        :root {
            --primary: #2563eb;
            --secondary: #1e40af;
            --accent: #3b82f6;
            --dark: #1f2937;
            --light: #f9fafb;
            --gray: #6b7280;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Typography */
        h1, h2, h3, h4 {
            line-height: 1.2;
            margin-bottom: 1rem;
            font-weight: 700;
        }
        
        h1 { font-size: 3rem; }
        h2 { font-size: 2.5rem; }
        h3 { font-size: 1.75rem; }
        
        p {
            margin-bottom: 1.5rem;
            color: var(--gray);
        }
        
        a {
            color: var(--primary);
            text-decoration: none;
            transition: var(--transition);
        }
        
        a:hover {
            color: var(--secondary);
        }
        
        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 0;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
        }
        
        .nav-links a {
            font-weight: 600;
            color: var(--dark);
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .hamburger {
            display: none;
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            padding: 10rem 0 5rem;
            text-align: center;
            background: linear-gradient(135deg, #f0f4ff 0%, #e6f0ff 100%);
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            margin: 0 auto 2rem;
            overflow: hidden;
            border: 5px solid white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .hero-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--primary);
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 50px;
            font-weight: 600;
            margin-top: 1rem;
            transition: var(--transition);
        }
        
        .cta-button:hover {
            background-color: var(--secondary);
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        /* About Section */
        .section {
            padding: 5rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary);
            margin: 1rem auto 0;
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1.5rem;
        }
        
        .skill-tag {
            background-color: #e0e7ff;
            color: var(--primary);
            padding: 0.25rem 0.75rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 600;
        }
        
        /* Portfolio Section */
        .portfolio {
            background-color: #f8fafc;
        }
        
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .portfolio-item {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: var(--transition);
        }
        
        .portfolio-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .portfolio-image {
            width: 100%;
            height: 200px;
            overflow: hidden;
        }
        
        .portfolio-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .portfolio-item:hover .portfolio-image img {
            transform: scale(1.05);
        }
        
        .portfolio-info {
            padding: 1.5rem;
        }
        
        .portfolio-category {
            display: inline-block;
            color: var(--primary);
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }
        
        /* Testimonials */
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .testimonial-card {
            background-color: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .testimonial-content {
            font-style: italic;
            margin-bottom: 1rem;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .author-image {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            overflow: hidden;
        }
        
        .author-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .author-name {
            font-weight: 600;
        }
        
        .author-title {
            font-size: 0.85rem;
            color: var(--gray);
        }
        
          /* Contact Section */
        #contact {
            text-align: center;
            padding: 40px 20px;
        }

        #contact h2 {
            color: #333;
            margin-bottom: 20px;
        }

        #contact h1 {
            color: #666;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        .contact-icons a {
            display: inline-block;
            margin: 0 10px;
            font-size: 1.5em;
            color: #555;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .contact-icons a:hover {
            color: #007bff;
        }

        
        input, textarea {
            width: 100%;
            padding: 0.75rem 1rem;
            border: 1px solid #e5e7eb;
            border-radius: 4px;
            font-family: inherit;
            font-size: 1rem;
            transition: var(--transition);
        }
        
        input:focus, textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.2);
        }
        
        textarea {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0;
            text-align: center;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 1.5rem 0;
        }
        
        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: rgba(255,255,255,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }
        
        .social-icon:hover {
            background-color: var(--primary);
        }
        
        .copyright {
            font-size: 0.85rem;
            color: rgba(255,255,255,0.7);
        }
        
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate {
            animation: fadeIn 0.8s ease forwards;
        }
        
        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        .delay-3 { animation-delay: 0.6s; }
        
        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background-color: white;
                flex-direction: column;
                align-items: center;
                padding: 2rem 0;
                gap: 2rem;
                transition: var(--transition);
            }
            
            .nav-links.active {
                left: 0;
            }
            
            .hamburger {
                display: block;
            }
            
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .hero {
                padding: 7rem 0 3rem;
            }
            
            .section {
                padding: 3rem 0;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M4 15s1-1 4-1 5 2 8 2 4-1 4-1V3s-1 1-4 1-5-2-8-2-4 1-4 1z"></path>
                        <line x1="4" y1="22" x2="4" y2="15"></line>
                    </svg>
                    MyPortofolio
                </a>
                
                <div class="nav-links" id="navLinks">
                    <a href="#home">Home</a>
                    <a href="#about">Tentang</a>
                    <a href="#portfolio">Portofolio</a>
                    <a href="#testimonials">Testimoni</a>
                    <a href="#contact">Kontak</a>
                </div>
                
                <div class="hamburger" id="hamburger">
                    <svg xmlns="c:\Users\kautzar\Documents\baru\WhatsApp Image 2025-06-29 at 20.27.20.jpeg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <line x1="3" y1="12" x2="21" y2="12"></line>
                        <line x1="3" y1="6" x2="21" y2="6"></line>
                        <line x1="3" y1="18" x2="21" y2="18"></line>
                    </svg>
                </div>
            </nav>
        </div>
    </header>
    
    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content animate">
                <div class="hero-image delay-1">
                    <img src="WhatsApp Image 2025-06-29 at 20.27.20.jpeg" />
                </div>
                <h1 class="delay-1">Hai, Saya Adji Pramudya Kautzar</h1>
                <h2 class="delay-2">Desainer & Pengembang Jaringan Kreatif</h2>
                <p class="delay-2">Saya membuat pengalaman digital yang indah, fungsional, dan berdampak untuk bisnis dan individu.</p>
                <a href="#portfolio" class="cta-button delay-3">Lihat Karya Saya</a>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section class="section" id="about">
        <div class="container">
            <h2 class="section-title">Tentang Saya</h2>
            
            <div class="about-content">
                <div class="animate">
                    <h3>Kreativitas adalah Passion Saya</h3>
                    <p>Dengan lebih dari 2 tahun pengalaman di industri digital, saya telah membantu berbagai klien dari setting hingga perusahaan besar mencapai tujuan online mereka melalui desain yang menarik dan solusi teknologi yang inovatif.</p>
                    <p>Saya percaya bahwa setiap proyek saya memberi kesempatan untuk menciptakan sesuatu yang istimewa yang tidak hanya memenuhi kebutuhan fungsional tetapi juga memberikan pengalaman pengguna yang luar biasa.</p>
                    
                    <div class="skills">
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">Html</span>
                        <span class="skill-tag">Css</span>
                        <span class="skill-tag">Mikrotik</span>
                        <span class="skill-tag">Editing Video</span>
                        <span class="skill-tag">Digital Marketing</span>
                        <span class="skill-tag">Desain canva</span>
                        <span class="skill-tag">Microsoft Office</span>
                        <span class="skill-tag">Ui/UX Figma</span>
                        <span class="skill-tag">Install Ulang</span>
                         <span class="skill-tag">Service Computer/laptop</span>

                    </div>
                </div>
                
                <div class="animate delay-1">
                    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/343cebd7-c2e3-4748-8494-9c2126e002e1.png" 
                             alt="Video thumbnail pekerjaan [Nama Anda], menunjukkan proses kreatif di depan komputer dengan kode dan desain di layar, suasana studio yang terang dan modern" 
                             style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: cover;">
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Portfolio Section -->
    <section class="section portfolio" id="portfolio">
        <div class="container">
            <h2 class="section-title">Karya Terbaru</h2>
            
            <div class="portfolio-grid">
                <!-- Item 1 -->
                <div class="portfolio-item animate">
                    <div class="portfolio-image">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/742d0174-4d2e-454a-acce-f7ec22a5a4f1.png" alt="Tampilan website e-commerce modern dengan layout bersih, warna biru dan putih, produk fashion ditampilkan secara menawan" />
                    </div>
                    <div class="portfolio-info">
                        <span class="portfolio-category">E-Commerce</span>
                        <h3>Fashion Store Redesign</h3>
                        <p>Redesign lengkap untuk toko fashion online dengan peningkatan UX dan conversion rate sebesar 40%.</p>
                        <a href="#" style="font-weight: 600;">Lihat Detail →</a>
                    </div>
                </div>
                
                <!-- Item 2 -->
                <div class="portfolio-item animate delay-1">
                    <div class="portfolio-image">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQt66Rj0ePstwKSyD7cV9ZAgMQ7Za3pqFCQlg&s"/>
                    </div>
                    <div class="portfolio-info">
                        <span class="portfolio-category">Microsoft Office</span>
                        <h3>Microsoft Office</h3>
                        <p>Tujuan utama dari Microsoft menciptakan layanan Office ini untuk memudahkan perkantoran.</p>
                        <a href="#" style="font-weight: 600;">Lihat Detail →</a>
                    </div>
                </div>
                
                <!-- Item 3 -->
                <div class="portfolio-item animate delay-2">
                    <div class="portfolio-image">
                        <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhDGit_oglIt5Dq4cc_ZXVXytMrPuvu8F15OxdvskT9fORuNhPN9uVt1NIOcBdXO9v3v7vM_N8OAoDdkvZczadsME87mQju6umVSUxLkyOcJw7KNpFOuaUt3DmPrQy1W-SuLds-KCGxLh0/s1600/setting-mikrotik-standart-1-line.jpg"/>
                    </div>
                    <div class="portfolio-info">
                        <span class="portfolio-category">Setting Mikrotik</span>
                        <h3>Setting mikrotik di sekolahan</h3>
                        <p>Mikrotik merupakan perangkat lunak, sekaligus sistem operasi yang dapat digunakan untuk menjadikan komputer dapat berfungsi sebagai network (jaringan), pengendali, atau pengatur lalu lintas antar jaringan komputer.</p>
                        <a href="#" style="font-weight: 600;">Lihat Detail →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials -->
    <section class="section" id="testimonials">
        <div class="container">
            <h2 class="section-title">Testimoni Klien</h2>
            
            <div class="testimonial-grid">
                <!-- Testimonial 1 -->
                <div class="testimonial-card animate">
                    <div class="testimonial-content">
                        <p>"Bekerja dengan adji pramudya kautzar adalah pengalaman yang luar biasa. Mereka benar-benar memahami visi kami dan menerjemahkannya ke dalam desain yang lebih baik dari yang kami harapkan."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-image">
                            <img src="image copy.png" />
                        </div>
                        <div>
                            <div class="author-name">Satria Sektiana</div>
                            <div class="author-title">CEO, Stria Store</div>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="testimonial-card animate delay-1">
                    <div class="testimonial-content">
                        <p>""Hasil kerja adji pramudya kautzar berdampak signifikan pada bisnis kami. Desainnya tidak hanya indah tapi juga fungsional, dengan peningkatan engagement yang nyata."
                    </div>
                    <div class="testimonial-author">
                        <div class="author-image">
                            <img src="image.png"/>
                        </div>
                        <div>
                            <div class="author-name">Cecilia</div>
                            <div class="author-title">Director of Marketing, Director of Marketing, Desain Grafis</div>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="testimonial-card animate delay-2">
                    <div class="testimonial-content">
                        <p>"Tim dan deadline sangat penting bagi kami. [Nama Anda] tidak hanya memenuhi target tapi juga memberikan solusi kreatif di luar ekspektasi."</p>
                    </div>
                    <div class="testimonial-author">
                        <div class="author-image">
                            <img src="image copy 2.png" />
                        </div>
                        <div>
                            <div class="author-name">fatimah az-zahra agustina lubis</div>
                            <div class="author-title">Kepala sekolah, Smk Darussalam</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
        </div>
    </section>
    <section id="contact" class="py-5 bg-light"> 
    </div>
    </section>
    <section id="contact" class="py-5 bg-light"> <div class="container">
            <h2 class="mb-4">Kontak</h2>
            <h1>085776689695</h2>
            <div class="contact-icons">
                </div>
               
            </div>
        </div>
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="logo" style="color: white; justify-content: center; margin-bottom: 1rem;">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <path d="M4 15s1-1 4-1 5 2 8 2 4-1 4-1V3s-1 1-4 1-5-2-8-2-4 1-4 1z"></path>
                    <line x1="4" y1="22" x2="4" y2="15"></line>
                </svg>
                MyPortofolio
            </div>
            
            <div class="social-links">
                <a href="https://www.linkedin.com/in/adji-kautzar-50b733281/" aria-label="LinkedIn Profile" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
                        <rect x="2" y="9" width="4" height="12"></rect>
                        <circle cx="4" cy="4" r="2"></circle>
                    </svg>
                </a>
                <a href="https://www.instagram.com/kautzar_354/" aria-label="Instagram Profile" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <circle cx="12" cy="12" r="10"></circle>
                        <path d="M8.56 2.75c4.37 6.03 6.02 9.42 8.03 17.72m2.54-15.38c-3.72 4.35-8.94 5.66-16.88 5.85m19.5 1.9c-3.5-.93-6.63-.82-8.94 0-2.58.92-5.01 2.86-7.44 6.32"></path>
                    </svg>
                </a>
                <a href="https://www.facebook.com/adji.kautzar.52?locale=id_ID" aria-label="facebook Profile" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <rect x="2" y="2" width="20" height="20" rx="2.18" ry="2.18"></rect>
                        <line x1="8" y1="12" x2="15" y2="12"></line>
                        <line x1="8" y1="8" x2="12" y2="8"></line>
                        <line x1="8" y1="16" x2="14" y2="16"></line>
                    </svg>
                </a>
                <a href="https://github.com/kautzaradji32" aria-label="GitHub Profile" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                    </svg>
                </a>
            </div>
            
            <p class="copyright">© 2023 Adji Pramudya Kautzar. All Rights Reserved.</p>
        </div>
    </footer>
    
    <script>
        // Mobile Navigation
        const hamburger = document.getElementById('hamburger');
        const navLinks = document.getElementById('navLinks');
        
        hamburger.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                navLinks.classList.remove('active');
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Animation on scroll
        const animateElements = document.querySelectorAll('.animate');
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, {
            threshold: 0.1
        });
        
        animateElements.forEach(element => {
            element.style.opacity = 0;
            element.style.transform = 'translateY(20px)';
            element.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            observer.observe(element);
        });
    </script>
</body>
</html>
