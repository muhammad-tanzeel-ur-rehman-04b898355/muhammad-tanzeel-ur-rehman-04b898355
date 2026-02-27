<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tanzeel Yousef | Full Stack Developer & WordPress Expert</title>
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <style>
        /* --- CSS Variables & Reset --- */
        :root {
            --primary-color: #3b82f6; /* Modern Blue */
            --secondary-color: #8b5cf6; /* Purple for React/Modern feel */
            --dark-bg: #0f172a;
            --card-bg: #1e293b;
            --text-light: #f8fafc;
            --text-gray: #94a3b8;
            --accent: #10b981; /* Green for success/growth */
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark-bg);
            color: var(--text-light);
            line-height: 1.6;
            overflow-x: hidden;
        }

        a { text-decoration: none; color: inherit; transition: 0.3s; }
        ul { list-style: none; }

        /* --- Components --- */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .btn {
            display: inline-block;
            padding: 12px 28px;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            border: 2px solid transparent;
        }

        .btn-primary {
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            color: white;
            box-shadow: 0 4px 15px rgba(59, 130, 246, 0.4);
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(59, 130, 246, 0.6);
        }

        .btn-outline {
            border-color: var(--primary-color);
            color: var(--primary-color);
            background: transparent;
        }

        .btn-outline:hover {
            background: var(--primary-color);
            color: white;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .section-subtitle {
            text-align: center;
            color: var(--text-gray);
            margin-bottom: 3rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* --- Header / Nav --- */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 15px 0;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--text-light);
        }
        .logo span { color: var(--primary-color); }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            color: var(--text-gray);
            font-size: 0.9rem;
            font-weight: 500;
        }

        .nav-links a:hover { color: var(--primary-color); }

        /* --- Hero Section --- */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding-top: 80px;
            background: radial-gradient(circle at center, #1e293b 0%, #0f172a 70%);
        }

        .hero-content h1 {
            font-size: 3.5rem;
            line-height: 1.2;
            margin-bottom: 20px;
        }

        .hero-content h1 span {
            color: var(--primary-color);
        }

        .hero-content p {
            font-size: 1.2rem;
            color: var(--text-gray);
            max-width: 700px;
            margin: 0 auto 30px;
        }

        .hero-badges {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .badge {
            background: rgba(59, 130, 246, 0.1);
            color: var(--primary-color);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid rgba(59, 130, 246, 0.3);
        }

        /* --- Journey Timeline (The Requested Feature) --- */
        .journey-section {
            padding: 100px 0;
            background: #162032;
        }

        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline::after {
            content: '';
            position: absolute;
            width: 4px;
            background-color: #334155;
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -2px;
            border-radius: 2px;
        }

        .timeline-item {
            padding: 10px 40px;
            position: relative;
            background-color: inherit;
            width: 50%;
        }

        .timeline-item::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            right: -10px;
            background-color: var(--dark-bg);
            border: 4px solid var(--primary-color);
            top: 15px;
            border-radius: 50%;
            z-index: 1;
        }

        .left { left: 0; }
        .right { left: 50%; }
        .left::before {
            content: " ";
            height: 0;
            position: absolute;
            top: 22px;
            width: 0;
            z-index: 1;
            right: 30px;
            border: medium solid white;
            border-width: 10px 0 10px 10px;
            border-color: transparent transparent transparent var(--card-bg);
        }
        .right::before {
            content: " ";
            height: 0;
            position: absolute;
            top: 22px;
            width: 0;
            z-index: 1;
            left: 30px;
            border: medium solid white;
            border-width: 10px 10px 10px 0;
            border-color: transparent var(--card-bg) transparent transparent;
        }
        .right::after { left: -10px; }

        .content-box {
            padding: 20px 30px;
            background-color: var(--card-bg);
            position: relative;
            border-radius: 6px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.3);
            border: 1px solid rgba(255,255,255,0.05);
        }

        .content-box h2 { color: var(--primary-color); margin-bottom: 5px; }
        .content-box .year { font-size: 0.85rem; color: var(--accent); font-weight: bold; margin-bottom: 10px; display: block;}
        .content-box p { font-size: 0.95rem; color: var(--text-gray); }

        /* --- Skills --- */
        .skills-section { padding: 100px 0; }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .skill-card {
            background: var(--card-bg);
            padding: 30px;
            border-radius: 12px;
            border: 1px solid rgba(255,255,255,0.05);
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary-color);
        }

        .skill-card i {
            font-size: 2.5rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
        }

        .skill-card h3 { margin-bottom: 15px; }
        
        .skill-tags span {
            display: inline-block;
            background: rgba(255,255,255,0.05);
            padding: 5px 10px;
            border-radius: 4px;
            font-size: 0.8rem;
            margin: 0 5px 8px 0;
            color: var(--text-gray);
        }

        /* --- Projects --- */
        .projects-section { padding: 100px 0; background: #162032; }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
        }

        .project-card {
            background: var(--card-bg);
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid rgba(255,255,255,0.05);
            transition: 0.3s;
        }

        .project-card:hover { transform: translateY(-5px); }

        .project-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            /* Placeholder styling since we use dynamic images */
            background-color: #334155;
        }

        .project-content { padding: 20px; }

        .project-content h3 { font-size: 1.2rem; margin-bottom: 10px; }
        .project-content p { font-size: 0.9rem; color: var(--text-gray); margin-bottom: 15px; }
        
        .tech-used {
            font-size: 0.8rem;
            color: var(--primary-color);
            margin-bottom: 15px;
            font-weight: 600;
        }

        .project-link {
            display: inline-block;
            color: var(--accent);
            font-size: 0.9rem;
            font-weight: 600;
        }
        .project-link:hover { text-decoration: underline; }

        /* --- Contact & Footer --- */
        .contact-section {
            padding: 100px 0;
            text-align: center;
        }

        .contact-cards {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 40px;
        }

        .contact-card {
            background: var(--card-bg);
            padding: 20px 30px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            gap: 15px;
            border: 1px solid rgba(255,255,255,0.05);
            transition: 0.3s;
        }
        
        .contact-card:hover {
            background: rgba(59, 130, 246, 0.1);
            border-color: var(--primary-color);
        }

        .contact-card i { font-size: 1.5rem; color: var(--primary-color); }
        .contact-card div { text-align: left; }
        .contact-card span { display: block; font-size: 0.8rem; color: var(--text-gray); }
        .contact-card strong { font-size: 1rem; }

        footer {
            background: #0b1120;
            padding: 30px 0;
            text-align: center;
            color: var(--text-gray);
            font-size: 0.9rem;
            border-top: 1px solid rgba(255,255,255,0.05);
        }

        /* --- Responsive Design --- */
        @media (max-width: 768px) {
            .hero-content h1 { font-size: 2.5rem; }
            .timeline::after { left: 31px; }
            .timeline-item { width: 100%; padding-left: 70px; padding-right: 25px; }
            .timeline-item::after { left: 21px; }
            .left::before, .right::before { left: 60px; border-width: 10px 10px 10px 0; border-color: transparent var(--card-bg) transparent transparent; }
            .right { left: 0; }
            .nav-links { display: none; } /* Simplified for single file */
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">Tanzeel<span>.dev</span></div>
                <ul class="nav-links">
                    <li><a href="#journey">My Journey</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <a href="#contact" class="btn btn-primary" style="padding: 8px 20px; font-size: 0.9rem;">Hire Me</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-badges">
                <span class="badge">Full Stack Developer</span>
                <span class="badge">React Expert</span>
                <span class="badge">WordPress Specialist</span>
            </div>
            <h1>From WordPress to <br><span>React Full Stack</span> Mastery</h1>
            <p>
                I started my journey customizing themes and plugins. Today, I build scalable, high-performance web applications with React, MySQL, and custom APIs. Bridging the gap between visual design and complex backend logic.
            </p>
            <div style="display: flex; gap: 15px; justify-content: center; flex-wrap: wrap;">
                <a href="#projects" class="btn btn-primary">View My Work</a>
                <a href="https://wa.me/923189046142" target="_blank" class="btn btn-outline"><i class="fab fa-whatsapp"></i> Chat on WhatsApp</a>
            </div>
        </div>
    </section>

    <!-- Journey Section (The Core Story) -->
    <section id="journey" class="journey-section">
        <div class="container">
            <h2 class="section-title">My Evolution</h2>
            <p class="section-subtitle">How a passion for building websites turned into a career in full-stack engineering.</p>
            
            <div class="timeline">
                <!-- Step 1 -->
                <div class="timeline-item left">
                    <div class="content-box">
                        <span class="year">The Beginning</span>
                        <h2>WordPress Expert</h2>
                        <p>Started with CMS. Mastered Elementor, Custom PHP, WooCommerce, and building 50+ custom sites. Learned the importance of SEO and user experience.</p>
                    </div>
                </div>
                <!-- Step 2 -->
                <div class="timeline-item right">
                    <div class="content-box">
                        <span class="year">Transition Phase</span>
                        <h2>Bootstrap & UI Development</h2>
                        <p>Wanted more control. Moved from drag-and-drop to writing code. Built responsive layouts with HTML5, CSS3, and Bootstrap.</p>
                    </div>
                </div>
                <!-- Step 3 -->
                <div class="timeline-item left">
                    <div class="content-box">
                        <span class="year">Modern Frontend</span>
                        <h2>React Developer</h2>
                        <p>Embraced the JavaScript ecosystem. Started building Single Page Applications (SPAs), interactive components, and consuming APIs with React.</p>
                    </div>
                </div>
                <!-- Step 4 -->
                <div class="timeline-item right">
                    <div class="content-box">
                        <span class="year">Current State</span>
                        <h2>Full Stack Engineer</h2>
                        <p>Completed the circle. Now creating robust Backends, managing MySQL Databases, and building secure REST APIs to power frontend applications.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills-section">
        <div class="container">
            <h2 class="section-title">Technical Expertise</h2>
            <p class="section-subtitle">A comprehensive toolkit for solving modern web challenges.</p>
            
            <div class="skills-grid">
                <!-- Frontend -->
                <div class="skill-card">
                    <i class="fab fa-react"></i>
                    <h3>Frontend Development</h3>
                    <p>Creating responsive, interactive, and pixel-perfect user interfaces.</p>
                    <div class="skill-tags">
                        <span>React.js</span>
                        <span>JavaScript (ES6+)</span>
                        <span>HTML5/CSS3</span>
                        <span>Bootstrap 5</span>
                        <span>Redux</span>
                    </div>
                </div>

                <!-- Backend -->
                <div class="skill-card">
                    <i class="fas fa-server"></i>
                    <h3>Backend & APIs</h3>
                    <p>Building logic, handling requests, and securing data flow.</p>
                    <div class="skill-tags">
                        <span>Node.js</span>
                        <span>RESTful APIs</span>
                        <span>Express</span>
                        <span>Custom PHP</span>
                    </div>
                </div>

                <!-- Database -->
                <div class="skill-card">
                    <i class="fas fa-database"></i>
                    <h3>Database Management</h3>
                    <p>Designing schemas and managing data efficiently.</p>
                    <div class="skill-tags">
                        <span>MySQL</span>
                        <span>Database Design</span>
                        <span>SQL Optimization</span>
                        <span>Data Migration</span>
                    </div>
                </div>

                <!-- CMS & Tools -->
                <div class="skill-card">
                    <i class="fab fa-wordpress"></i>
                    <h3>CMS & Platforms</h3>
                    <p>Leveraging platforms for rapid business solutions.</p>
                    <div class="skill-tags">
                        <span>WordPress Customization</span>
                        <span>WooCommerce</span>
                        <span>Elementor Pro</span>
                        <span>Shopify</span>
                        <span>Go High Level</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects-section">
        <div class="container">
            <h2 class="section-title">Featured Projects</h2>
            <p class="section-subtitle">A selection of complex builds spanning from custom CMS solutions to Full Stack apps.</p>
            
            <div class="projects-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/car/400/250" alt="Exchange My Car" class="project-img">
                    <div class="project-content">
                        <h3>Exchange My Car</h3>
                        <div class="tech-used">Custom PHP | Frontend Optimization</div>
                        <p>A complex car exchange platform with advanced search filters, user authentication, and seamless vehicle listing management.</p>
                        <a href="https://www.exchangemycar.co.uk/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/pet/400/250" alt="The Pet Smart" class="project-img">
                    <div class="project-content">
                        <h3>The Pet Smart</h3>
                        <div class="tech-used">WooCommerce | WordPress</div>
                        <p>Complete e-commerce pet store with inventory management, local delivery integration, and payment gateways.</p>
                        <a href="https://thepetsmart.pk/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/tech/400/250" alt="Collab Culture" class="project-img">
                    <div class="project-content">
                        <h3>Collab Culture</h3>
                        <div class="tech-used">Go High Level | Directory</div>
                        <p>A custom-coded directory website connecting creative professionals with advanced search and messaging systems.</p>
                        <a href="https://collabculture.ca/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/auto/400/250" alt="Car Adviser" class="project-img">
                    <div class="project-content">
                        <h3>Car Adviser</h3>
                        <div class="tech-used">WordPress | Custom PHP | ULEZ</div>
                        <p>Automotive advice site featuring ULEZ map integration and vehicle compliance checks for UK users.</p>
                        <a href="https://www.caradviser.co.uk/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 5 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/spa/400/250" alt="Kijiji Spa" class="project-img">
                    <div class="project-content">
                        <h3>Kijiji Spa</h3>
                        <div class="tech-used">WordPress | Booking System</div>
                        <p>Elegant spa website with online booking functionality, service showcase, and tranquil design.</p>
                        <a href="https://kijijispa.com/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 6 -->
                <div class="project-card">
                    <img src="https://picsum.photos/seed/job/400/250" alt="Go Woda" class="project-img">
                    <div class="project-content">
                        <h3>Go Woda</h3>
                        <div class="tech-used">WordPress | Job Portal</div>
                        <p>Custom job portal with employer dashboards, application tracking, and profile management.</p>
                        <a href="https://gowoda.com/" target="_blank" class="project-link">View Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 40px;">
                <a href="#" class="btn btn-outline">View All 50+ Projects</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="container">
            <h2 class="section-title">Let's Work Together</h2>
            <p class="section-subtitle">Ready to bring your project to life? Reach out via any platform below.</p>

            <div class="contact-cards">
                <!-- WhatsApp -->
                <a href="https://wa.me/923189046142" target="_blank" class="contact-card">
                    <i class="fab fa-whatsapp"></i>
                    <div>
                        <span>WhatsApp</span>
                        <strong>+92 318 9046142</strong>
                    </div>
                </a>

                <!-- Fiverr -->
                <a href="https://www.fiverr.com/s/Q7LvY03" target="_blank" class="contact-card">
                    <i class="fab fa-fiverr"></i>
                    <div>
                        <span>Fiverr</span>
                        <strong>Hire on Fiverr</strong>
                    </div>
                </a>

                <!-- Upwork -->
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?mp_source=share" target="_blank" class="contact-card">
                    <i class="fab fa-upwork"></i>
                    <div>
                        <span>Upwork</span>
                        <strong>Upwork Profile</strong>
                    </div>
                </a>

                <!-- Email -->
                <a href="mailto:mtwebexperts.site@gmail.com" class="contact-card">
                    <i class="fas fa-envelope"></i>
                    <div>
                        <span>Email</span>
                        <strong>mtwebexperts.site</strong>
                    </div>
                </a>
                
                 <!-- LinkedIn -->
                 <a href="https://www.linkedin.com/in/muhammad-tanzeel-ur-rehman-04b898355/" target="_blank" class="contact-card">
                    <i class="fab fa-linkedin"></i>
                    <div>
                        <span>LinkedIn</span>
                        <strong>Connect Professional</strong>
                    </div>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Tanzeel Yousef. WordPress Expert & Full Stack Developer.</p>
            <p style="font-size: 0.8rem; margin-top: 10px; opacity: 0.6;">Designed with Passion for Professional Excellence</p>
        </div>
    </footer>

</body>
</html>
