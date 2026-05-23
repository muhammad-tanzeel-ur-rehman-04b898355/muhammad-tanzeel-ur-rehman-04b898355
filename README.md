<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tanzeel Yousef | Full Stack PHP & WordPress Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: #1a1a2e;
            line-height: 1.6;
            padding: 2rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 2rem;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
            padding: 2rem;
        }

        h1 {
            font-size: 2.5rem;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 0.5rem;
        }

        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
            margin: 1rem 0 1.5rem;
        }

        .badge {
            display: inline-block;
            padding: 0.4rem 1rem;
            border-radius: 2rem;
            font-size: 0.85rem;
            font-weight: 600;
            text-decoration: none;
            transition: transform 0.2s;
        }

        .badge:hover {
            transform: translateY(-2px);
        }

        .badge-portfolio { background: #000; color: white; }
        .badge-linkedin { background: #0077b5; color: white; }
        .badge-fiverr { background: #1dbf73; color: white; }
        .badge-upwork { background: #14a800; color: white; }

        .rate {
            display: inline-block;
            background: #10b981;
            color: white;
            padding: 0.3rem 1rem;
            border-radius: 2rem;
            font-weight: bold;
            margin-left: 1rem;
            font-size: 1rem;
        }

        .section {
            margin: 2.5rem 0;
        }

        .section-title {
            font-size: 1.8rem;
            font-weight: 700;
            border-left: 5px solid #667eea;
            padding-left: 1rem;
            margin-bottom: 1.5rem;
            color: #1e293b;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 1rem;
            margin: 1.5rem 0;
        }

        .stat-card {
            background: #f1f5f9;
            padding: 1rem;
            text-align: center;
            border-radius: 1rem;
            font-weight: bold;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 800;
            color: #667eea;
        }

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .card {
            background: #f8fafc;
            padding: 1.25rem;
            border-radius: 1rem;
            border-left: 4px solid #667eea;
        }

        .card h3 {
            color: #1e293b;
            margin-bottom: 0.75rem;
        }

        .card ul {
            list-style: none;
            padding-left: 0;
        }

        .card li {
            padding: 0.25rem 0;
            padding-left: 1.2rem;
            position: relative;
        }

        .card li::before {
            content: "✔";
            position: absolute;
            left: 0;
            color: #10b981;
        }

        .tech-table {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            background: #f1f5f9;
            padding: 1.5rem;
            border-radius: 1rem;
        }

        .tech-category {
            font-weight: 700;
            color: #475569;
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin: 1.5rem 0;
        }

        .project-card {
            background: #ffffff;
            border: 1px solid #e2e8f0;
            border-radius: 1rem;
            overflow: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 24px rgba(0,0,0,0.1);
        }

        .project-preview {
            background: #f1f5f9;
            height: 140px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            border-bottom: 1px solid #e2e8f0;
        }

        .project-info {
            padding: 1rem;
        }

        .project-title {
            font-weight: 800;
            color: #1e293b;
            margin-bottom: 0.5rem;
        }

        .project-link {
            display: inline-block;
            margin-top: 0.75rem;
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
        }

        .project-link:hover {
            text-decoration: underline;
        }

        .contact {
            background: #1e293b;
            color: white;
            padding: 2rem;
            border-radius: 1.5rem;
            text-align: center;
        }

        .contact a {
            color: #a5f3fc;
            text-decoration: none;
        }

        .footer-quote {
            text-align: center;
            font-style: italic;
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 2px solid #e2e8f0;
            color: #475569;
        }

        @media (max-width: 768px) {
            body {
                padding: 1rem;
            }
            .container {
                padding: 1rem;
            }
            h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
<div class="container">
    
    <!-- Header -->
    <h1>👋 Hi, I'm Tanzeel Yousef</h1>
    <div>
        🚀 <strong>Available for Hire</strong> 
        <span class="rate">💲 $5.00/hr</span>
    </div>
    
    <div class="badge-container">
        <a href="https://tanzeel-yousef.netlify.app" class="badge badge-portfolio">🌐 Portfolio</a>
        <a href="https://www.linkedin.com/in/muhammad-tanzeel-ur-rehman-04b898355/" class="badge badge-linkedin">🔗 LinkedIn</a>
        <a href="https://www.fiverr.com/tanzeelyousef96" class="badge badge-fiverr">💰 Fiverr</a>
        <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8" class="badge badge-upwork">📌 Upwork</a>
    </div>

    <p>I am a <strong>Full Stack PHP Developer & WordPress Expert</strong> with 3+ years of experience building modern, responsive, and high-performance web solutions for businesses worldwide. I specialize in creating scalable, secure, and user-friendly platforms — from custom PHP applications to advanced WordPress ecosystems.</p>

    <!-- Stats -->
    <div class="stats-grid">
        <div class="stat-card"><div class="stat-number">50+</div> Projects Delivered</div>
        <div class="stat-card"><div class="stat-number">3+</div> Years Experience</div>
        <div class="stat-card"><div class="stat-number">20+</div> Happy Clients</div>
        <div class="stat-card"><div class="stat-number">30+</div> Migrations</div>
        <div class="stat-card"><div class="stat-number">60%</div> Avg Speed Gain</div>
    </div>

    <!-- Journey -->
    <div class="section">
        <div class="section-title">💼 My Journey</div>
        <p>My development journey began with <strong>WordPress</strong>, where I successfully delivered <strong>50+ projects</strong>, mastering custom themes, WooCommerce, API integrations, performance tuning, and SEO.</p><br>
        <p>Evolving into a <strong>Full Stack PHP Developer</strong>, I now architect and build complete web systems:</p>
        <ul style="margin: 1rem 0 0 2rem;">
            <li>🧩 Custom PHP & MySQL Applications (Admin panels, dashboards, backend logic)</li>
            <li>⚛️ Modern Frontends (HTML5, CSS3, JavaScript, Bootstrap)</li>
            <li>🔌 Advanced WordPress with ACF Pro & Elementor Pro</li>
            <li>🛍️ WooCommerce Stores with custom checkout & payment gateways</li>
            <li>⚡ Performance & SEO Optimization (Core Web Vitals, caching, technical SEO)</li>
        </ul>
        <p style="margin-top: 1rem;">Today, I deliver end-to-end web solutions tailored to business goals — combining robust backend engineering with engaging user experiences.</p>
    </div>

    <!-- Core Expertise -->
    <div class="section">
        <div class="section-title">🛠 Core Expertise</div>
        <div class="expertise-grid">
            <div class="card"><h3>🔹 Full Stack PHP</h3><ul><li>Custom web apps from scratch</li><li>Secure PHP & MySQL architecture</li><li>Admin panels & dashboards</li><li>API integrations</li></ul></div>
            <div class="card"><h3>🔹 WordPress Development</h3><ul><li>Custom themes & functionality</li><li>ACF Pro Specialist</li><li>Elementor & Elementor Pro Expert</li><li>Plugin customization</li></ul></div>
            <div class="card"><h3>🔹 WooCommerce</h3><ul><li>Store setup & payment gateways</li><li>Inventory & order automation</li><li>Custom checkout experiences</li></ul></div>
            <div class="card"><h3>🔹 Frontend</h3><ul><li>HTML5, CSS3, JavaScript, Bootstrap</li><li>Responsive, mobile-first design</li><li>Pixel-perfect Figma to code</li></ul></div>
            <div class="card"><h3>🔹 Performance & SEO</h3><ul><li>Core Web Vitals optimization</li><li>Caching & minification</li><li>Technical SEO & Schema Markup</li></ul></div>
        </div>
    </div>

    <!-- Tech Stack -->
    <div class="section">
        <div class="section-title">⚙️ Tech Stack</div>
        <div class="tech-table">
            <div><span class="tech-category">🎨 Frontend:</span> HTML5, CSS3, JavaScript, Bootstrap</div>
            <div><span class="tech-category">⚙️ Backend:</span> PHP, MySQL, REST APIs</div>
            <div><span class="tech-category">📦 CMS:</span> WordPress, WooCommerce, Elementor Pro, ACF Pro</div>
            <div><span class="tech-category">🛠️ Tools:</span> Git, GitHub, VS Code, Netlify, NPM</div>
        </div>
    </div>

    <!-- Experience -->
    <div class="section">
        <div class="section-title">🏢 Professional Experience</div>
        <div class="card" style="margin-bottom: 1rem;">
            <h3>Full Stack PHP & WordPress Developer</h3>
            <p><strong>East & West Web Development and SEO Agency</strong> | Pakistan (Remote) | 2022 – Present</p>
            <ul><li>50+ custom WordPress & PHP projects globally</li><li>Dynamic sites with ACF Pro & Elementor Pro</li><li>WooCommerce + Stripe/PayPal integration</li><li>60% speed & Core Web Vitals improvement</li></ul>
        </div>
        <div class="card">
            <h3>WordPress Developer & Full Stack Developer</h3>
            <p><strong>TECH BITS IT</strong> | Dera Ismail Khan | April 2021 – 2022</p>
            <ul><li>Custom WordPress & WooCommerce solutions</li><li>Payment gateways & membership systems</li><li>Vehicle registration & ULEZ detection systems</li><li>Advanced booking platforms</li></ul>
        </div>
    </div>

    <!-- Education -->
    <div class="section">
        <div class="section-title">🎓 Education</div>
        <p><strong>Bachelor of Science in Computer Science</strong> (In Progress)<br>Hayat Medical College | 2025</p>
    </div>

    <!-- Featured Projects (Upwork) -->
    <div class="section">
        <div class="section-title">📁 Featured Work</div>
        <p><em>Click any project card to view full details on Upwork ↓</em></p>
        <div class="project-grid">
            <div class="project-card">
                <div class="project-preview">📄</div>
                <div class="project-info">
                    <div class="project-title">Custom ACF Pro Build</div>
                    <p>Dynamic content system for business directory</p>
                    <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2058092268697952256" target="_blank" class="project-link">View Project →</a>
                </div>
            </div>
            <div class="project-card">
                <div class="project-preview">🎨</div>
                <div class="project-info">
                    <div class="project-title">Elementor Pro Website</div>
                    <p>Pixel-perfect responsive business site</p>
                    <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2058090236860235776" target="_blank" class="project-link">View Project →</a>
                </div>
            </div>
            <div class="project-card">
                <div class="project-preview">🛒</div>
                <div class="project-info">
                    <div class="project-title">WooCommerce Store</div>
                    <p>Full e-commerce with payment integration</p>
                    <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2058078963023663104" target="_blank" class="project-link">View Project →</a>
                </div>
            </div>
            <div class="project-card">
                <div class="project-preview">⚡</div>
                <div class="project-info">
                    <div class="project-title">Performance Optimization</div>
                    <p>Core Web Vitals & speed boost</p>
                    <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2058078248599298048" target="_blank" class="project-link">View Project →</a>
                </div>
            </div>
        </div>
        <details>
            <summary style="cursor: pointer; font-weight: 600; margin-top: 1rem;">📂 View all 20+ Upwork projects</summary>
            <div style="margin-top: 1rem; display: flex; flex-wrap: wrap; gap: 0.5rem;">
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2058075277836689408" target="_blank">Project 5</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992545424934248448" target="_blank">Project 6</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1934543359322857472" target="_blank">Project 7</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=2002628008675958784" target="_blank">Project 8</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1934545994476752896" target="_blank">Project 9</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992449779213099008" target="_blank">Project 10</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992544840567037952" target="_blank">Project 11</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992544214992355328" target="_blank">Project 13</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992543282387574784" target="_blank">Project 15</a> • 
                <a href="https://www.upwork.com/freelancers/~019473e56b1a594fa8?p=1992456132622700544" target="_blank">Project 20</a>
            </div>
        </details>
    </div>

    <!-- Why choose me -->
    <div class="section">
        <div class="section-title">🌟 Why Clients Choose Me</div>
        <ul style="columns: 2; column-gap: 2rem; list-style: none; padding-left: 0;">
            <li>✅ 50+ successful international projects</li>
            <li>✅ Strong PHP & WordPress core expertise</li>
            <li>✅ Advanced ACF Pro & Elementor Pro skills</li>
            <li>✅ Complex, custom web applications</li>
            <li>✅ Reliable communication & on-time delivery</li>
            <li>✅ Business-focused, scalable solutions</li>
        </ul>
    </div>

    <!-- Contact -->
    <div class="contact">
        <h3 style="color: white;">📬 Let's Connect</h3>
        <p>📧 <a href="mailto:mtanzeelxen@gmail.com">mtanzeelxen@gmail.com</a> &nbsp;|&nbsp; 📱 WhatsApp: 0318-9046142</p>
        <p>📍 Dera Ismail Khan, Pakistan &nbsp;|&nbsp; 🌐 <a href="https://tanzeel-yousef.netlify.app">tanzeel-yousef.netlify.app</a></p>
    </div>

    <!-- Quote -->
    <div class="footer-quote">
        💬 “First, solve the problem. Then, write the code.” — John Johnson
    </div>

</div>
</body>
</html>
