# Guia: Como Criar um Portfólio HTML para Freelancers

Um portfólio online é essencial para desenvolvedores freelancers. Neste guia, você aprenderá a criar um portfólio completo, responsivo e profissional usando HTML, CSS e JavaScript.

## 📋 Índice

1. [Introdução](#introdução)
2. [Estrutura de Arquivos](#estrutura-de-arquivos)
3. [HTML Base](#html-base)
4. [CSS Moderno](#css-moderno)
5. [JavaScript Interativo](#javascript-interativo)
6. [SEO Básico](#seo-básico)
7. [Publicação](#publicação)
8. [Exemplo Completo](#exemplo-completo)

---

## 🎯 Introdução

Um portfólio online mostra suas habilidades, projetos e experiências. Para freelancers, é uma vitrine 24/7 que atrai clientes.

### Por que ter um portfólio?

- **Visibilidade:** Aparece em buscas do Google
- **Credibilidade:** Mostra profissionalismo
- **Conversão:** Gera leads e oportunidades
- **Controle:** Você decide como apresentar seu trabalho

---

## 📁 Estrutura de Arquivos

```
portfolio/
├── index.html          # Página principal
├── css/
│   └── style.css       # Estilos
├── js/
│   └── script.js       # Interatividade
├── images/             # Fotos e ícones
└── README.md
```

---

## 🏗️ HTML Base

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio - Desenvolvedor Freelancer</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="logo">DevFreela</div>
            <nav class="nav">
                <ul class="nav-list" id="navList">
                    <li><a href="#home" class="nav-link">Início</a></li>
                    <li><a href="#about" class="nav-link">Sobre</a></li>
                    <li><a href="#services" class="nav-link">Serviços</a></li>
                    <li><a href="#projects" class="nav-link">Projetos</a></li>
                    <li><a href="#contact" class="nav-link">Contato</a></li>
                </ul>
                <button class="nav-toggle" id="navToggle">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Olá! Eu sou <span class="highlight">Desenvolvedor Full Stack</span></h1>
            <p>Crio soluções web modernas e eficientes para negócios como o seu.</p>
            <a href="#contact" class="btn btn-primary">Vamos conversar?</a>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <h2>Sobre Mim</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Sou desenvolvedor full stack com 5+ anos de experiência em projetos web e mobile. Especializado em React, Node.js e MongoDB.</p>
                    <div class="skills">
                        <span class="skill">React</span>
                        <span class="skill">Node.js</span>
                        <span class="skill">TypeScript</span>
                        <span class="skill">MongoDB</span>
                        <span class="skill">AWS</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2>Serviços</h2>
            <div class="services-grid">
                <div class="service-card">
                    <h3>Desenvolvimento Web</h3>
                    <p>Sites e aplicações web responsivas e performáticas.</p>
                </div>
                <div class="service-card">
                    <h3>API REST</h3>
                    <p>APIs robustas e seguras para integração de sistemas.</p>
                </div>
                <div class="service-card">
                    <h3>Manutenção</h3>
                    <p>Correção de bugs e otimização de performance.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="projects" id="projects">
        <div class="container">
            <h2>Projetos</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>Gerenciador de Tarefas</h3>
                    <p>Aplicação full stack para gestão de tarefas com autenticação.</p>
                    <a href="#" class="project-link">Ver projeto →</a>
                </div>
                <div class="project-card">
                    <h3>E-commerce Personalizado</h3>
                    <p>Loja virtual completa com pagamento e gestão de estoque.</p>
                    <a href="#" class="project-link">Ver projeto →</a>
                </div>
                <div class="project-card">
                    <h3>Dashboard de Analytics</h3>
                    <p>Painel de controle com gráficos e métricas em tempo real.</p>
                    <a href="#" class="project-link">Ver projeto →</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2>Contato</h2>
            <form class="contact-form" id="contactForm">
                <div class="form-group">
                    <input type="text" id="name" required placeholder="Seu nome">
                </div>
                <div class="form-group">
                    <input type="email" id="email" required placeholder="Seu e-mail">
                </div>
                <div class="form-group">
                    <textarea id="message" required placeholder="Sua mensagem"></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Enviar Mensagem</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2024 DevFreela. Todos os direitos reservados.</p>
            <div class="social-links">
                <a href="#">LinkedIn</a>
                <a href="#">GitHub</a>
                <a href="#">Twitter</a>
            </div>
        </div>
    </footer>

    <script src="js/script.js"></script>
</body>
</html>
```

---

## 🎨 CSS Moderno

```css
/* css/style.css */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary: #0066ff;
    --primary-dark: #0052cc;
    --text: #333;
    --text-light: #666;
    --bg: #ffffff;
    --bg-light: #f8f9fa;
    --border: #e1e5e9;
}

body {
    font-family: 'Inter', sans-serif;
    color: var(--text);
    background: var(--bg);
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header */
.header {
    position: sticky;
    top: 0;
    background: var(--bg);
    border-bottom: 1px solid var(--border);
    z-index: 100;
}

.header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 0;
}

.logo {
    font-size: 24px;
    font-weight: 700;
    color: var(--primary);
}

.nav {
    display: flex;
    align-items: center;
}

.nav-list {
    display: flex;
    list-style: none;
    gap: 30px;
}

.nav-link {
    text-decoration: none;
    color: var(--text);
    font-weight: 500;
    transition: color 0.3s;
}

.nav-link:hover {
    color: var(--primary);
}

.nav-toggle {
    display: none;
    flex-direction: column;
    background: none;
    border: none;
    cursor: pointer;
    gap: 4px;
}

.nav-toggle span {
    width: 25px;
    height: 3px;
    background: var(--text);
    transition: all 0.3s;
}

/* Hero */
.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    background: linear-gradient(135deg, #f0f4ff 0%, #ffffff 100%);
    padding: 80px 0;
}

.hero h1 {
    font-size: 3.5rem;
    margin-bottom: 20px;
    line-height: 1.2;
}

.highlight {
    color: var(--primary);
}

.hero p {
    font-size: 1.25rem;
    color: var(--text-light);
    margin-bottom: 30px;
    max-width: 600px;
}

.btn {
    display: inline-block;
    padding: 12px 30px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s;
    border: none;
    cursor: pointer;
    font-size: 16px;
}

.btn-primary {
    background: var(--primary);
    color: white;
}

.btn-primary:hover {
    background: var(--primary-dark);
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0, 102, 255, 0.3);
}

/* Sections */
section {
    padding: 80px 0;
}

section h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 60px;
    position: relative;
}

section h2::after {
    content: '';
    position: absolute;
    bottom: -15px;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 4px;
    background: var(--primary);
    border-radius: 2px;
}

/* About */
.about-content {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 40px;
    align-items: center;
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 20px;
}

.skill {
    background: var(--bg-light);
    padding: 8px 16px;
    border-radius: 20px;
    font-size: 14px;
    font-weight: 500;
}

/* Services */
.services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.service-card {
    background: var(--bg-light);
    padding: 30px;
    border-radius: 12px;
    text-align: center;
    transition: transform 0.3s;
}

.service-card:hover {
    transform: translateY(-5px);
}

.service-card h3 {
    color: var(--primary);
    margin-bottom: 15px;
}

/* Projects */
.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.project-card {
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 25px;
    transition: box-shadow 0.3s;
}

.project-card:hover {
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.project-link {
    color: var(--primary);
    text-decoration: none;
    font-weight: 600;
    display: inline-block;
    margin-top: 15px;
}

/* Contact */
.contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: grid;
    gap: 20px;
}

.form-group {
    display: flex;
    flex-direction: column;
}

.form-group input,
.form-group textarea {
    padding: 15px;
    border: 2px solid var(--border);
    border-radius: 8px;
    font-family: inherit;
    font-size: 16px;
    transition: border-color 0.3s;
}

.form-group input:focus,
.form-group textarea:focus {
    outline: none;
    border-color: var(--primary);
}

/* Footer */
.footer {
    background: #1a1a1a;
    color: white;
    text-align: center;
    padding: 40px 0;
}

.social-links {
    margin-top: 15px;
    display: flex;
    justify-content: center;
    gap: 20px;
}

.social-links a {
    color: white;
    text-decoration: none;
    opacity: 0.7;
    transition: opacity 0.3s;
}

.social-links a:hover {
    opacity: 1;
}

/* Responsive */
@media (max-width: 768px) {
    .nav-list {
        position: fixed;
        top: 0;
        right: -100%;
        height: 100vh;
        width: 70%;
        max-width: 300px;
        background: var(--bg);
        flex-direction: column;
        align-items: center;
        padding-top: 80px;
        gap: 30px;
        transition: right 0.3s;
    }

    .nav-list.active {
        right: 0;
    }

    .nav-toggle {
        display: flex;
    }

    .hero h1 {
        font-size: 2.5rem;
    }

    .about-content {
        grid-template-columns: 1fr;
    }

    section {
        padding: 60px 0;
    }
}
```

---

## ⚡ JavaScript Interativo

```javascript
// js/script.js

// Mobile Navigation Toggle
const navToggle = document.getElementById('navToggle');
const navList = document.getElementById('navList');

navToggle.addEventListener('click', () => {
    navList.classList.toggle('active');
});

// Smooth Scroll
document.querySelectorAll('.nav-link').forEach(link => {
    link.addEventListener('click', e => {
        e.preventDefault();
        const target = document.querySelector(link.getAttribute('href'));
        if (target) {
            target.scrollIntoView({ behavior: 'smooth' });
            navList.classList.remove('active');
        }
    });
});

// Form Validation
const contactForm = document.getElementById('contactForm');

if (contactForm) {
    contactForm.addEventListener('submit', e => {
        e.preventDefault();
        
        const name = document.getElementById('name').value.trim();
        const email = document.getElementById('email').value.trim();
        const message = document.getElementById('message').value.trim();

        if (!name || !email || !message) {
            alert('Por favor, preencha todos os campos.');
            return;
        }

        if (!isValidEmail(email)) {
            alert('Por favor, insira um e-mail válido.');
            return;
        }

        // Simula envio
        alert('Mensagem enviada com sucesso! Retornaremos em breve.');
        contactForm.reset();
    });
}

function isValidEmail(email) {
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return emailRegex.test(email);
}

// Scroll Animation
const observerOptions = {
    threshold: 0.1
};

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
            entry.target.style.transform = 'translateY(0)';
        }
    });
}, observerOptions);

// Observe sections
document.querySelectorAll('section').forEach(section => {
    section.style.opacity = '0';
    section.style.transform = 'translateY(20px)';
    section.style.transition = 'all 0.6s ease';
    observer.observe(section);
});
```

---

## 🔍 SEO Básico

Adicione estas tags no `<head>` do seu HTML:

```html
<!-- SEO Básico -->
<meta name="description" content="Portfólio de desenvolvedor full stack especializado em React, Node.js e MongoDB. Veja meus projetos e entre em contato.">
<meta name="keywords" content="desenvolvedor, freelancer, React, Node.js, MongoDB, portfólio">
<meta name="author" content="Seu Nome">

<!-- Open Graph -->
<meta property="og:title" content="Portfólio - Seu Nome">
<meta property="og:description" content="Desenvolvedor full stack freelancer">
<meta property="og:image" content="URL_DA_SUA_IMAGEM">
<meta property="og:url" content="URL_DO_SEU_PORTFOLIO">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
```

---

## 🚀 Publicação

### GitHub Pages (Gratuito)

1. Crie um repositório no GitHub
2. Faça upload dos arquivos
3. Vá em Settings → Pages
4. Selecione a branch `main`
5. Pronto! Seu site estará em `https://seu-usuario.github.io/nome-repo/`

### Netlify (Gratuito)

1. Acesse [netlify.com](https://netlify.com)
2. Conecte sua conta do GitHub
3. Selecione o repositório
4. Configure: Build command: (deixe vazio), Publish directory: `/`
5. Clique em Deploy site

### Vercel (Gratuito)

1. Acesse [vercel.com](https://vercel.com)
2. Conecte sua conta do GitHub
3. Importe o repositório
4. Clique em Deploy

---

## 📦 Exemplo Completo

Para um exemplo pronto e funcional, clone este repositório:

```bash
git clone https://github.com/hermestwogetherbot/portfolio-html-guide.git
```

---

## 📝 Dicas Finais

1. **Mantenha simples:** Foque em 3-5 projetos de qualidade
2. **Carregamento rápido:** Otimize imagens (use WebP)
3. **Mobile primeiro:** Teste em dispositivos reais
4. **Atualize regularmente:** Adicione novos projetos
5. **Call to action:** Tenha botões de contato visíveis
6. **Teste:** Peça feedback de outros desenvolvedores

## 🤝 Contribuição

Sinta-se à vontade para abrir issues ou pull requests com melhorias!

## 📄 Licença

Este projeto está sob a licença MIT.