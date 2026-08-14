<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Portfolio</title>
    <style>
        :root {
            --bg-color: #0d1117;
            --card-bg: #161b22;
            --border-color: #30363d;
            --text-primary: #c9d1d9;
            --text-secondary: #8b949e;
            --accent-color: #58a6ff;
            --accent-hover: #1f6feb;
            --tag-bg: #21262d;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            line-height: 1.6;
        }

        header {
            background-color: rgba(22, 27, 34, 0.8);
            backdrop-filter: blur(10px);
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 100;
            border-bottom: 1px solid var(--border-color);
        }

        nav {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        nav .logo {
            font-weight: bold;
            font-size: 1.2rem;
            color: var(--accent-color);
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        nav a {
            color: var(--text-primary);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.2s;
        }

        nav a:hover {
            color: var(--accent-color);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 6rem 2rem 3rem 2rem;
        }

        section {
            margin-bottom: 5rem;
        }

        /* Hero Section */
        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            min-height: 60vh;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
        }

        .hero h1 span {
            color: var(--accent-color);
        }

        .hero p {
            font-size: 1.25rem;
            color: var(--text-secondary);
            max-width: 700px;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent-color);
            color: #ffffff;
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.2s;
            width: fit-content;
        }

        .btn:hover {
            background-color: var(--accent-hover);
        }

        /* Section Titles */
        .section-title {
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 0.5rem;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .skill-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 1.5rem;
        }

        .skill-card h3 {
            margin-bottom: 1rem;
            color: var(--accent-color);
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tag {
            background-color: var(--tag-bg);
            border: 1px solid var(--border-color);
            padding: 0.3rem 0.6rem;
            border-radius: 4px;
            font-size: 0.85rem;
            color: var(--text-primary);
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .project-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transition: transform 0.2s;
        }

        .project-card:hover {
            transform: translateY(-4px);
        }

        .project-card h3 {
            margin-bottom: 0.5rem;
        }

        .project-card p {
            color: var(--text-secondary);
            font-size: 0.95rem;
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            border-top: 1px solid var(--border-color);
            color: var(--text-secondary);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo">DEVA MITHRAN</div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <div class="container">
        
        <!-- Hero Section -->
        <section class="hero" id="about">
            <h1>Hi, I'm <span>Software & Hardware Developer</span></h1>
            <p>I build low-level systems, develop applications in RUST & C++, and work with embedded microcontrollers like Arduino and rasberry pi. Passionate about hardware architecture and OS customization and mainly work with arch linux and bare kernals.</p>
            <a href="#projects" class="btn">View My Work</a>
        </section>

        <!-- Skills Section -->
        <section id="skills">
            <h2 class="section-title">Skills & Technologies</h2>
            <div class="skills-grid">
                
                <div class="skill-card">
                    <h3>Languages</h3>
                    <div class="tags">
                        <span class="tag">C++</span>
                        <span class="tag">bash</span>
                        <span class="tag">RUST</span>
                        <span class="tag">C</span>
                        <span class="tag">HTML/CSS</span>
                    </div>
                </div>

                <div class="skill-card">
                    <h3>Hardware & IoT</h3>
                    <div class="tags">
                        <span class="tag">Arduino</span>
                        <span class="tag">Rassberry pi</span>
                        <span class="tag">handhelds and wearables</span>
                        <span class="tag">Circuit Prototyping</span>
                    </div>
                </div>

                <div class="skill-card">
                    <h3>Systems & Tools</h3>
                    <div class="tags">
                        <span class="tag">Arch Linux</span>
                        <span class="tag">Android Customization</span>
                        <span class="tag">Git</span>
                        <span class="tag">Vercel</span>
                    </div>
                </div>

            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2 class="section-title">Featured Projects</h2>
            <div class="projects-grid">

                <div class="project-card">
                    <div>
                        <h3>Arduino gaming</h3>
                        <p>Arm aurdino chip powered by dragonwing,i installed arch in it and played steam games </p>
                    </div>
                    <div class="tags">
                        <span class="tag">C++</span>
                        <span class="tag">Arduino</span>
                        <span class="tag">Hardware</span>
                    </div>
                </div>

                <div class="project-card">
                    <div>
                        <h3>OS Logic & System Utilities</h3>
                        <p>Command-line software utilities exploring low-level operating system simulations, task logic, and performance calculators.</p>
                    </div>
                    <div class="tags">
                        <span class="tag">C++</span>
                        <span class="tag">RUST</span>
                    </div>
                </div>

                <div class="project-card">
                    <div>
                        <h3>Game Utilities & Custom Launchers</h3>
                        <p>Custom scripts and mod management utilities designed for game optimization and custom launchers.</p>
                    </div>
                    <div class="tags">
                        <span class="tag">Python</span>
                        <span class="tag">System Scripts</span>
                         <span class="tag">Unreal engine</span>
                    </div>
                </div>

            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2 class="section-title">Get In Touch</h2>
            <p style="color: var(--text-secondary); margin-bottom: 1.5rem;">Interested in collaborating or talking about hardware & software development?</p>
            <a href="https://github.com/devamithran87-dot" target="_blank" class="btn">Connect on GitHub</a>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 Developer Portfolio. Hosted on GitHub Pages.</p>
    </footer>

</body>
</html>
