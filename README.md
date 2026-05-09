<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chelak Gatbel | Portfolio</title>
    <style>
        :root {
            --bg: #050505;
            --card: #111111;
            --accent: #6366f1;
            --text: #ffffff;
            --text-dim: #a1a1aa;
            --border: #27272a;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { 
            font-family: 'Inter', -apple-system, sans-serif; 
            background: var(--bg); 
            color: var(--text); 
            line-height: 1.6; 
            padding: 0 20px;
        }

        .container { max-width: 900px; margin: 0 auto; }

        /* Header */
        header { padding: 80px 0 40px; text-align: center; }
        h1 { font-size: 3rem; font-weight: 800; letter-spacing: -2px; margin-bottom: 10px; }
        .subtitle { color: var(--accent); font-weight: 600; letter-spacing: 2px; text-transform: uppercase; font-size: 0.8rem; }

        /* Sections */
        section { padding: 40px 0; }
        h2 { font-size: 1.5rem; margin-bottom: 24px; display: flex; align-items: center; gap: 10px; }
        h2::after { content: ""; height: 1px; background: var(--border); flex: 1; }

        /* Skills Grid */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 15px;
        }
        .skill-item {
            background: var(--card);
            border: 1px solid var(--border);
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            font-weight: 500;
            transition: 0.3s;
        }
        .skill-item:hover { border-color: var(--accent); transform: translateY(-3px); }

        /* Projects Grid */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }
        .project-card {
            background: var(--card);
            border: 1px solid var(--border);
            border-radius: 12px;
            padding: 24px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .project-card h3 { margin-bottom: 10px; color: var(--accent); }
        .project-card p { color: var(--text-dim); font-size: 0.95rem; margin-bottom: 20px; }
        .tech-stack { display: flex; gap: 8px; flex-wrap: wrap; }
        .tag { font-size: 0.75rem; background: #1e1e22; padding: 4px 10px; border-radius: 4px; color: #818cf8; }

        /* Contact */
        .contact-box {
            background: linear-gradient(145deg, #111, #050505);
            border: 1px solid var(--accent);
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            margin-bottom: 60px;
        }
        .email-btn {
            display: inline-block;
            margin-top: 20px;
            background: var(--accent);
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
        }

        @media (max-width: 600px) {
            h1 { font-size: 2.2rem; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <p class="subtitle">Full-Stack Developer</p>
            <h1>Chelak Gatbel</h1>
        </header>

        <section id="skills">
            <h2>Technical Skills</h2>
            <div class="skills-container">
                <div class="skill-item">React.js</div>
                <div class="skill-item">Node.js</div>
                <div class="skill-item">JavaScript (ES6+)</div>
                <div class="skill-item">HTML5 / CSS3</div>
                <div class="skill-item">MongoDB</div>
                <div class="skill-item">Three.js</div>
                <div class="skill-item">WebGPU</div>
                <div class="skill-item">Git / GitHub</div>
            </div>
        </section>

        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <div>
                        <h3>Inventory Manager</h3>
                        <p>A smart system to track stock levels with automated total value calculation based on unit pricing.</p>
                    </div>
                    <div class="tech-stack">
                        <span class="tag">JavaScript</span>
                        <span class="tag">Local Storage</span>
                    </div>
                </div>

                <div class="project-card">
                    <div>
                        <h3>3D Media Browser</h3>
                        <p>An immersive media explorer utilizing Three.js and WebGPU for high-performance rendering.</p>
                    </div>
                    <div class="tech-stack">
                        <span class="tag">Three.js</span>
                        <span class="tag">WebGPU</span>
                    </div>
                </div>

                <div class="project-card">
                    <div>
                        <h3>SocialConnect</h3>
                        <p>A social media interface featuring real-time feed simulations and interactive user profiles.</p>
                    </div>
                    <div class="tech-stack">
                        <span class="tag">React</span>
                        <span class="tag">Node.js</span>
                    </div>
                </div>
            </div>
        </section>

        <section class="contact-box">
            <h2>Let's Work Together</h2>
            <p>Currently available for freelance projects or full-time roles.</p>
            <a href="mailto:chelakgatbel19@gmail.com" class="email-btn">Hire Me</a>
            <p style="margin-top: 15px; color: var(--text-dim);">chelakgatbel19@gmail.com</p>
        </section>

        <footer style="text-align: center; padding-bottom: 40px; color: var(--text-dim); font-size: 0.8rem;">
            &copy; 2026 Chelak Gatbel. Built with precision.
        </footer>
    </div>

</body>
</html>
