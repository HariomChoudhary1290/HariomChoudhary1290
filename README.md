<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hariom Choudhary - DevOps Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            overflow-x: hidden;
        }

        /* Animated Background Particles */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
            pointer-events: none;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: rgba(255, 255, 255, 0.6);
            border-radius: 50%;
            animation: float 15s infinite ease-in-out;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) translateX(0); opacity: 0; }
            10% { opacity: 1; }
            90% { opacity: 1; }
            100% { transform: translateY(-100vh) translateX(50px); opacity: 0; }
        }

        .container {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Hero Section with 3D Card */
        .hero {
            text-align: center;
            margin-bottom: 60px;
            perspective: 1000px;
        }

        .hero-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 30px;
            padding: 60px 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            transform-style: preserve-3d;
            transition: transform 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .hero-card:hover {
            transform: rotateY(5deg) rotateX(5deg);
        }

        .profile-img-container {
            width: 200px;
            height: 200px;
            margin: 0 auto 30px;
            position: relative;
            animation: float-profile 3s ease-in-out infinite;
        }

        @keyframes float-profile {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .profile-img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 5px solid #4CAF50;
            box-shadow: 0 10px 40px rgba(76, 175, 80, 0.5);
            object-fit: cover;
        }

        .glow-ring {
            position: absolute;
            top: -10px;
            left: -10px;
            right: -10px;
            bottom: -10px;
            border-radius: 50%;
            border: 3px solid transparent;
            border-top-color: #4CAF50;
            border-right-color: #4CAF50;
            animation: rotate 3s linear infinite;
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            background: linear-gradient(45deg, #fff, #4CAF50);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradient-shift 3s ease infinite;
        }

        @keyframes gradient-shift {
            0%, 100% { filter: hue-rotate(0deg); }
            50% { filter: hue-rotate(20deg); }
        }

        .tagline {
            font-size: 1.3em;
            margin-top: 20px;
            opacity: 0.9;
        }

        /* 3D Floating Cards */
        .section {
            margin-bottom: 50px;
        }

        .section-title {
            font-size: 2.5em;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
            display: inline-block;
            width: 100%;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, transparent, #4CAF50, transparent);
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            perspective: 1000px;
        }

        .card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transform-style: preserve-3d;
            animation: card-float 3s ease-in-out infinite;
        }

        .card:nth-child(2) {
            animation-delay: 0.5s;
        }

        .card:nth-child(3) {
            animation-delay: 1s;
        }

        @keyframes card-float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .card:hover {
            transform: translateY(-15px) rotateX(10deg);
            box-shadow: 0 20px 50px rgba(76, 175, 80, 0.4);
            border-color: #4CAF50;
        }

        .card h3 {
            font-size: 1.8em;
            margin-bottom: 15px;
            color: #4CAF50;
        }

        .card p, .card ul {
            line-height: 1.8;
            opacity: 0.9;
        }

        .card ul {
            list-style: none;
            padding-left: 0;
        }

        .card ul li {
            padding: 8px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .card ul li:last-child {
            border-bottom: none;
        }

        /* Skills Section with 3D Pills */
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .skill-pill {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(5px);
            padding: 12px 25px;
            border-radius: 30px;
            font-size: 1.1em;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
            transform-style: preserve-3d;
            cursor: pointer;
        }

        .skill-pill:hover {
            background: #4CAF50;
            transform: translateY(-5px) scale(1.1);
            box-shadow: 0 10px 25px rgba(76, 175, 80, 0.5);
        }

        /* Social Buttons with 3D Effect */
        .social-buttons {
            display: flex;
            gap: 20px;
            justify-content: center;
            margin-top: 40px;
        }

        .social-btn {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            padding: 15px 35px;
            border-radius: 15px;
            text-decoration: none;
            color: #fff;
            font-weight: bold;
            font-size: 1.1em;
            transition: all 0.3s ease;
            border: 2px solid rgba(255, 255, 255, 0.3);
            display: inline-block;
            transform-style: preserve-3d;
        }

        .social-btn:hover {
            background: #4CAF50;
            border-color: #4CAF50;
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 35px rgba(76, 175, 80, 0.5);
        }

        .footer {
            text-align: center;
            margin-top: 60px;
            padding: 30px;
            background: rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
            border-radius: 20px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            h1 { font-size: 2.5em; }
            .section-title { font-size: 2em; }
            .card-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <!-- Animated Particles Background -->
    <div class="particles" id="particles"></div>

    <div class="container">
        <!-- Hero Section -->
        <div class="hero">
            <div class="hero-card">
                <div class="profile-img-container">
                    <div class="glow-ring"></div>
                    <img src="https://ui-avatars.com/api/?name=Hariom+Choudhary&size=200&background=4CAF50&color=fff&bold=true" 
                         alt="Hariom Choudhary" 
                         class="profile-img">
                </div>
                <h1>👋 Hi, I'm Hariom Choudhary</h1>
                <p class="tagline">
                    <strong>I believe Cloud & DevOps is for EVERYONE — yes, YOU TOO!<br>
                    Join me on my journey 🚀</strong>
                </p>
            </div>
        </div>

        <!-- About Section -->
        <div class="section">
            <h2 class="section-title">👨‍💻 About Me</h2>
            <div class="card-grid">
                <div class="card">
                    <h3>💼 Role</h3>
                    <p>DevOps Engineer passionate about automation and cloud infrastructure</p>
                </div>
                <div class="card">
                    <h3>🎯 Mission</h3>
                    <p>Helping beginners start their DevOps career and solving real-world problems</p>
                </div>
                <div class="card">
                    <h3>📚 Growth</h3>
                    <p>Always learning, always improving, always building scalable systems</p>
                </div>
            </div>
        </div>

        <!-- Contact Section -->
        <div class="section">
            <h2 class="section-title">📞 Contact Details</h2>
            <div class="card-grid">
                <div class="card">
                    <h3>📩 Email</h3>
                    <p>hariom.choudhary015@gmail.com</p>
                </div>
                <div class="card">
                    <h3>📱 Phone</h3>
                    <p>9584581290</p>
                </div>
                <div class="card">
                    <h3>🔗 LinkedIn</h3>
                    <p>linkedin.com/in/hariom-choudhary-868823322</p>
                </div>
            </div>
        </div>

        <!-- Skills Section -->
        <div class="section">
            <h2 class="section-title">⚙️ DevOps Skills</h2>
            <div class="skills-container">
                <div class="skill-pill">GitHub Actions</div>
                <div class="skill-pill">Jenkins</div>
                <div class="skill-pill">Docker</div>
                <div class="skill-pill">Kubernetes</div>
                <div class="skill-pill">Terraform</div>
                <div class="skill-pill">Ansible</div>
                <div class="skill-pill">AWS</div>
                <div class="skill-pill">Prometheus</div>
                <div class="skill-pill">Grafana</div>
                <div class="skill-pill">Git</div>
                <div class="skill-pill">Linux</div>
            </div>
        </div>

        <!-- Technologies Section -->
        <div class="section">
            <h2 class="section-title">🚀 Technologies</h2>
            <div class="card">
                <ul>
                    <li><strong>CI/CD:</strong> GitHub Actions, Jenkins</li>
                    <li><strong>Containers:</strong> Docker, Docker Compose</li>
                    <li><strong>Orchestration:</strong> Kubernetes</li>
                    <li><strong>IaC:</strong> Terraform, Ansible</li>
                    <li><strong>Cloud:</strong> AWS (EC2, IAM, S3, VPC, Lambda)</li>
                    <li><strong>Monitoring:</strong> Prometheus, Grafana</li>
                    <li><strong>Version Control:</strong> Git, GitHub</li>
                    <li><strong>OS:</strong> Linux (Ubuntu, CentOS)</li>
                </ul>
            </div>
        </div>

        <!-- Social Links -->
        <div class="social-buttons">
            <a href="https://linkedin.com/in/hariom-choudhary-868823322" class="social-btn" target="_blank">
                LinkedIn
            </a>
            <a href="mailto:hariom.choudhary015@gmail.com" class="social-btn">
                Email Me
            </a>
        </div>

        <!-- Footer -->
        <div class="footer">
            <p>Made with ❤️ by <strong>Hariom Choudhary</strong></p>
        </div>
    </div>

    <script>
        // Create animated particles
        const particlesContainer = document.getElementById('particles');
        for (let i = 0; i < 50; i++) {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.animationDelay = Math.random() * 15 + 's';
            particle.style.animationDuration = (Math.random() * 10 + 10) + 's';
            particlesContainer.appendChild(particle);
        }

        // 3D Card tilt effect on mouse move
        const heroCard = document.querySelector('.hero-card');
        heroCard.addEventListener('mousemove', (e) => {
            const rect = heroCard.getBoundingClientRect();
            const x = e.clientX - rect.left;
            const y = e.clientY - rect.top;
            
            const centerX = rect.width / 2;
            const centerY = rect.height / 2;
            
            const rotateX = (y - centerY) / 20;
            const rotateY = (centerX - x) / 20;
            
            heroCard.style.transform = `rotateX(${rotateX}deg) rotateY(${rotateY}deg)`;
        });

        heroCard.addEventListener('mouseleave', () => {
            heroCard.style.transform = 'rotateX(0) rotateY(0)';
        });
    </script>
</body>
</html>
