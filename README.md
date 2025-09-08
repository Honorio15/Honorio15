<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Honório Neto - Desenvolvedor</title>
    <style>
        :root {
            --primary: #2b2d42;
            --secondary: #8d99ae;
            --accent: #ef233c;
            --light: #edf2f4;
            --dark: #1d1f2c;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--primary);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 30px 0;
            flex-wrap: wrap;
        }
        
        .profile {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        
        .profile-pic {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--accent);
        }
        
        .profile-info h1 {
            font-size: 2.5rem;
            margin-bottom: 5px;
        }
        
        .profile-info p {
            color: var(--secondary);
            font-size: 1.2rem;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }
        
        .social-links a {
            color: var(--primary);
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--accent);
        }
        
        section {
            margin: 40px 0;
        }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--secondary);
        }
        
        .about {
            background-color: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .skill-category h3 {
            margin-bottom: 10px;
            color: var(--accent);
        }
        
        .skill-list {
            list-style: none;
        }
        
        .skill-list li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }
        
        .project-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-content {
            padding: 20px;
        }
        
        .project-content h3 {
            margin-bottom: 10px;
            color: var(--accent);
        }
        
        .project-content p {
            margin-bottom: 15px;
            color: var(--secondary);
        }
        
        .tech-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 15px 0;
        }
        
        .tech-tag {
            background-color: var(--primary);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
        }
        
        .project-links {
            display: flex;
            gap: 15px;
        }
        
        .project-links a {
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 5px;
            transition: color 0.3s;
        }
        
        .project-links a:hover {
            color: var(--accent);
        }
        
        .github-stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .stat-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .stat-card h3 {
            font-size: 2rem;
            color: var(--accent);
        }
        
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
            color: var(--secondary);
            border-top: 1px solid #ddd;
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }
            
            .profile {
                flex-direction: column;
            }
            
            .social-links {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile">
                <img src="https://avatars.githubusercontent.com/u/106992006?v=4" alt="Honório Neto" class="profile-pic">
                <div class="profile-info">
                    <h1>Honório Neto</h1>
                    <p>Desenvolvedor Python | Ciência de Dados | Aprendizado de Máquina</p>
                    <div class="social-links">
                        <a href="https://github.com/Honorio15" target="_blank" title="GitHub">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="https://www.linkedin.com/in/honorioneto/" target="_blank" title="LinkedIn">
                            <i class="fab fa-linkedin"></i>
                        </a>
                        <a href="mailto:honorioneto1510@gmail.com" title="Email">
                            <i class="fas fa-envelope"></i>
                        </a>
                    </div>
                </div>
            </div>
        </header>

        <section class="about">
            <h2>Sobre Mim</h2>
            <p>Olá! Sou Honório Neto, um desenvolvedor apaixonado por tecnologia e soluções inovadoras. Atualmente, estou focado em desenvolvimento Python, ciência de dados e aprendizado de máquina. Estou constantemente aprendendo novas tecnologias e melhorando minhas habilidades para criar soluções que impactem positivamente a vida das pessoas.</p>
            <p>Além do desenvolvimento de software, tenho interesse em inteligência artificial, automação e desenvolvimento web. Estou sempre aberto a colaborar em projetos interessantes e desafiadores.</p>
        </section>

        <section>
            <h2>Habilidades Técnicas</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Linguagens de Programação</h3>
                    <ul class="skill-list">
                        <li>Python</li>
                        <li>JavaScript</li>
                        <li>Java</li>
                        <li>C</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Desenvolvimento Web</h3>
                    <ul class="skill-list">
                        <li>HTML & CSS</li>
                        <li>React</li>
                        <li>Node.js</li>
                        <li>Flask</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Ciência de Dados & ML</h3>
                    <ul class="skill-list">
                        <li>Pandas</li>
                        <li>NumPy</li>
                        <li>Scikit-learn</li>
                        <li>TensorFlow</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Ferramentas & Outros</h3>
                    <ul class="skill-list">
                        <li>Git & GitHub</li>
                        <li>SQL</li>
                        <li>Docker</li>
                        <li>Linux</li>
                    </ul>
                </div>
            </div>
        </section>

        <section>
            <h2>Projetos em Destaque</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-content">
                        <h3>Previsão de Preços de Imóveis</h3>
                        <p>Sistema de machine learning para prever valores de imóveis com base em características como localização, tamanho e amenities.</p>
                        <div class="tech-list">
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">Scikit-learn</span>
                            <span class="tech-tag">Pandas</span>
                        </div>
                        <div class="project-links">
                            <a href="#"><i class="fas fa-code"></i> Código</a>
                            <a href="#"><i class="fas fa-external-link-alt"></i> Demo</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-content">
                        <h3>Sistema de Automação</h3>
                        <p>Ferramenta de automação de tarefas repetitivas usando Python e Selenium para otimizar processos empresariais.</p>
                        <div class="tech-list">
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">Selenium</span>
                            <span class="tech-tag">Automation</span>
                        </div>
                        <div class="project-links">
                            <a href="#"><i class="fas fa-code"></i> Código</a>
                            <a href="#"><i class="fas fa-external-link-alt"></i> Demo</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-content">
                        <h3>App de Gestão Financeira</h3>
                        <p>Aplicativo web para controle de finanças pessoais com visualizações de gastos e receitas.</p>
                        <div class="tech-list">
                            <span class="tech-tag">React</span>
                            <span class="tech-tag">Node.js</span>
                            <span class="tech-tag">MongoDB</span>
                        </div>
                        <div class="project-links">
                            <a href="#"><i class="fas fa-code"></i> Código</a>
                            <a href="#"><i class="fas fa-external-link-alt"></i> Demo</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section>
            <h2>Estatísticas do GitHub</h2>
            <div class="github-stats">
                <div class="stat-card">
                    <h3>20+</h3>
                    <p>Repositórios</p>
                </div>
                <div class="stat-card">
                    <h3>15+</h3>
                    <p>Projetos Concluídos</p>
                </div>
                <div class="stat-card">
                    <h3>100+</h3>
                    <p>Contribuições</p>
                </div>
                <div class="stat-card">
                    <h3>3</h3>
                    <p>Linguagens</p>
                </div>
            </div>
        </section>

        <footer>
            <p>© 2023 Honório Neto. Todos os direitos reservados.</p>
            <p>📧 honoriohneto@gmail.com</p>
        </footer>
    </div>

    <!-- Font Awesome para ícones -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
