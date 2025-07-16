<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio - Desenvolvedor Full Stack</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light-color);
            color: var(--dark-color);
            line-height: 1.6;
        }
        
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
            position: relative;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: white;
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--secondary-color);
        }
        
        .hero {
            padding: 4rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        .skills {
            padding: 4rem 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2rem;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .skill-card {
            background-color: var(--light-color);
            padding: 1.5rem;
            border-radius: 5px;
            text-align: center;
            transition: transform 0.3s;
        }
        
        .skill-card:hover {
            transform: translateY(-10px);
        }
        
        .skill-card i {
            font-size: 3rem;
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        
        .projects {
            padding: 4rem 0;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background-color: white;
            border-radius: 5px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .project-image {
            height: 200px;
            background-color: #ddd;
            position: relative;
        }
        
        .project-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .project-info {
            padding: 1.5rem;
        }
        
        .project-info h3 {
            margin-bottom: 1rem;
        }
        
        .project-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .contact {
            padding: 4rem 0;
            background-color: var(--primary-color);
            color: white;
        }
        
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 0.8rem;
            border-radius: 5px;
            border: none;
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            background-color: var(--dark-color);
            color: white;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-bottom: 1rem;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--secondary-color);
        }
        
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <div class="logo">MeuPortfólio</div>
                <div class="nav-links">
                    <a href="#skills">Habilidades</a>
                    <a href="#projects">Projetos</a>
                    <a href="#certificates">Certificados</a>
                    <a href="#contact">Contato</a>
                </div>
            </nav>
            
            <div class="hero">
                <h1>Olá, eu sou [Yago Chan]</h1>
                <p>Desenvolvedor Full Stack com experiência em JavaScript, Python, Java e diversos frameworks modernos. Apaixonado por criar soluções inovadoras e eficientes.</p>
                <a href="#contact" class="btn">Entre em Contato</a>
            </div>
        </div>
    </header>
    
    <section id="skills" class="skills">
        <div class="container">
            <h2 class="section-title">Minhas Habilidades</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <i class="fab fa-js"></i>
                    <h3>JavaScript</h3>
                    <p>Desenvolvimento front-end e back-end com Node.js, experiência com React e outros frameworks.</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-python"></i>
                    <h3>Python</h3>
                    <p>Desenvolvimento back-end com Django e Flask, análise de dados e automação.</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-java"></i>
                    <h3>Java</h3>
                    <p>Desenvolvimento de aplicações empresariais e sistemas robustos.</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-database"></i>
                    <h3>Banco de Dados</h3>
                    <p>MySQL, MongoDB e PostgreSQL - modelagem e consultas complexas.</p>
                </div>
                <div class="skill-card">
                    <i class="fab fa-git-alt"></i>
                    <h3>Controle de Versão</h3>
                    <p>Git e GitHub - colaboração eficiente em projetos de equipe.</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-code-branch"></i>
                    <h3>Metodologias Ágeis</h3>
                    <p>Scrum, Kanban - entrega contínua de valor em projetos.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="projects" class="projects">
        <div class="container">
            <h2 class="section-title">Meus Projetos</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://placehold.co/600x400" alt="Sistema de gerenciamento de tarefas com React, Node.js e MongoDB">
                    </div>
                    <div class="project-info">
                        <h3>Sistema de Gerenciamento de Tarefas</h3>
                        <p>Aplicação full stack para organização de tarefas com autenticação de usuário e banco de dados em tempo real.</p>
                        <div class="project-links">
                            <a href="#" class="btn">Ver Projeto</a>
                            <a href="#" class="btn">Código Fonte</a>
                        </div>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://placehold.co/600x400" alt="API RESTful para e-commerce desenvolvida com Python e Django REST framework">
                    </div>
                    <div class="project-info">
                        <h3>API RESTful para E-commerce</h3>
                        <p>Back-end completo para plataforma de comércio eletrônico com autenticação JWT e documentação Swagger.</p>
                        <div class="project-links">
                            <a href="#" class="btn">Ver Projeto</a>
                            <a href="#" class="btn">Código Fonte</a>
                        </div>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                        <img src="https://placehold.co/600x400" alt="Aplicativo mobile de finanças pessoais desenvolvido com React Native">
                    </div>
                    <div class="project-info">
                        <h3>Aplicativo de Finanças Pessoais</h3>
                        <p>Aplicativo mobile para controle de gastos e planejamento financeiro com gráficos interativos.</p>
                        <div class="project-links">
                            <a href="#" class="btn">Ver Projeto</a>
                            <a href="#" class="btn">Código Fonte</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="certificates" class="skills">
        <div class="container">
            <h2 class="section-title">Meus Certificados</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <i class="fas fa-certificate"></i>
                    <h3>JavaScript Developer</h3>
                    <p>Certificado em desenvolvimento JavaScript avançado pela W3Schools.</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-certificate"></i>
                    <h3>Python PCEP</h3>
                    <p>Certificado de Programador Python de Nível Básico pelo Python Institute.</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-certificate"></i>
                    <h3>React Developer</h3>
                    <p>Certificação em desenvolvimento com React pela Coursera.</p>
                </div>
                <div class="skill-card">
                    <i class="fas fa-certificate"></i>
                    <h3>MongoDB Certified</h3>
                    <p>Certificado de Desenvolvedor MongoDB Associate.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Entre em Contato</h2>
            <form class="contact-form">
                <div class="form-group">
                    <label for="name">Nome</label>
                    <input type="text" id="name" placeholder="Seu nome">
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" placeholder="seu@email.com">
                </div>
                <div class="form-group">
                    <label for="message">Mensagem</label>
                    <textarea id="message" rows="5" placeholder="Sua mensagem"></textarea>
                </div>
                <button type="submit" class="btn">Enviar Mensagem</button>
            </form>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
            </div>
            <p>&copy; 2023 [Seu Nome]. Todos os direitos reservados.</p>
        </div>
    </footer>
    
    <script>
        // Efeito de rolagem suave
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Formulário de contato (simulação)
        const form = document.querySelector('.contact-form');
        form.addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Mensagem enviada com sucesso! Em breve entrarei em contato.');
            form.reset();
        });
    </script>
</body>
</html>
