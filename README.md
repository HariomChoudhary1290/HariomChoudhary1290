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
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        /* Profile Section */
        .profile-section {
            background: white;
            border-radius: 20px;
            padding: 40px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            margin-bottom: 30px;
            animation: fadeIn 0.6s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid #4CAF50;
            margin-bottom: 20px;
            animation: bounce 2s ease-in-out infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        h1 {
            font-size: 2.5em;
            color: #667eea;
            margin-bottom: 10px;
        }

        .tagline {
            color: #666;
            font-size: 1.1em;
            margin-top: 15px;
        }

        /* Cards */
        .card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        h2 {
            color: #667eea;
            font-size: 1.8em;
            margin-bottom: 20px;
            border-bottom: 3px solid #4CAF50;
            padding-bottom: 10px;
            display: inline-block;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }

        .info-item {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid #4CAF50;
        }

        .info-item strong {
            color: #667eea;
            display: block;
            margin-bottom: 5px;
        }

        /* Skills */
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }

        .skill {
            background: #667eea;
            color: white;
            padding: 10px 20px;
            border-radius: 20px;
            font-size: 0.9em;
            transition: all 0.3s ease;
        }

        .skill:hover {
            background: #4CAF50;
            transform: scale(1.1);
        }

        /* Social Links */
        .social-links {
            display: flex;
            gap: 15px;
            justify-content: center;
            margin-top: 30px;
        }

        .social-btn {
            background: #667eea;
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            display: inline-block;
        }

        .social-btn:hover {
            background: #4CAF50;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(76, 175, 80, 0.4);
        }

        .footer {
            text-align: center;
            color: white;
            margin-top: 40px;
            padding: 20px;
        }

        /* About List */
        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            padding: 10px 0;
            color: #555;
            line-height: 1.6;
        }

        ul li:before {
            content: "✓ ";
            color: #4CAF50;
            font-weight: bold;
            margin-right: 10px;
        }

        @media (max-width: 768px) {
            h1 { font-size: 2em; }
            .profile-section { padding: 30px 20px; }
            .card { padding: 20px; }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Profile Section -->
        <div class="profile-section">
            <img src="https://ui-avatars.com/api/?name=Hariom+Choudhary&size=150&background=4CAF50&color=fff&bold=true" 
                 alt="Hariom Choudhary" 
                 class="profile-img">
            <h1>👋 Hi, I'm Hariom Choudhary</h1>
            <p><strong>DevOps Engineer</strong></p>
            <p class="tagline">I believe Cloud & DevOps is for EVERYONE — yes, YOU TOO!<br>
            Join me on my journey 🚀</p>
        </div>

        <!-- About Me -->
        <div class="card">
            <h2>👨‍💻 About Me</h2>
            <ul>
                <li>DevOps Engineer passionate about Cloud & Automation</li>
                <li>Love solving real-world problems & building scalable systems</li>
                <li>Helping beginners start their DevOps career</li>
                <li>Always learning, always improving</li>
            </ul>
        </div>

        <!-- Contact Details -->
        <div class="card">
            <h2>📞 Contact Details</h2>
            <div class="info-grid">
                <div class="info-item">
                    <strong>📩 Email</strong>
                    hariom.choudhary015@gmail.com
                </div>
                <div class="info-item">
                    <strong>📱 Phone</strong>
                    9584581290
                </div>
                <div class="info-item">
                    <strong>🔗 LinkedIn</strong>
                    hariom-choudhary-868823322
                </div>
            </div>
        </div>

        <!-- DevOps Skills -->
        <div class="card">
            <h2>⚙️ DevOps Skills</h2>
            <div class="skills">
                <span class="skill">GitHub Actions</span>
                <span class="skill">Jenkins</span>
                <span class="skill">Docker</span>
                <span class="skill">Kubernetes</span>
                <span class="skill">Terraform</span>
                <span class="skill">Ansible</span>
                <span class="skill">AWS</span>
                <span class="skill">Prometheus</span>
                <span class="skill">Grafana</span>
                <span class="skill">Git</span>
                <span class="skill">Linux</span>
            </div>
        </div>

        <!-- Technologies -->
        <div class="card">
            <h2>🚀 Technologies</h2>
            <div class="info-grid">
                <div class="info-item">
                    <strong>CI/CD</strong>
                    GitHub Actions, Jenkins
                </div>
                <div class="info-item">
                    <strong>Containers</strong>
                    Docker, Docker Compose
                </div>
                <div class="info-item">
                    <strong>Orchestration</strong>
                    Kubernetes
                </div>
                <div class="info-item">
                    <strong>IaC</strong>
                    Terraform, Ansible
                </div>
                <div class="info-item">
                    <strong>Cloud</strong>
                    AWS (EC2, IAM, S3, VPC, Lambda)
                </div>
                <div class="info-item">
                    <strong>Monitoring</strong>
                    Prometheus, Grafana
                </div>
                <div class="info-item">
                    <strong>Version Control</strong>
                    Git, GitHub
                </div>
                <div class="info-item">
                    <strong>OS</strong>
                    Linux (Ubuntu, CentOS)
                </div>
            </div>
        </div>

        <!-- Social Links -->
        <div class="social-links">
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
</body>
</html>
