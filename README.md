# portifolio-fron-end-html-css-javascript
 Construindo seu Portfólio Front-end do Zero com HTML, CSS e JavaScript
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <h1>Meu Portfólio</h1>
        <nav>
            <ul>
                <li><a href="#about">Sobre Mim</a></li>
                <li><a href="#projects">Projetos</a></li>
                <li><a href="#contact">Contato</a></li>
            </ul>
        </nav>
    </header>
    <section id="about" class="about">
        <h2>Sobre Mim</h2>
        <p>Olá! Sou um desenvolvedor front-end apaixonado por criar interfaces incríveis e responsivas.</p>
    </section>
    <section id="projects" class="projects">
        <h2>Meus Projetos</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>Projeto 1</h3>
                <img src="path/to/project1-image.jpg" alt="Imagem do Projeto 1">
                <p>Descrição do Projeto 1.</p>
            </div>
            <div class="project-card">
                <h3>Projeto 2</h3>
                <img src="path/to/project2-image.jpg" alt="Imagem do Projeto 2">
                <p>Descrição do Projeto 2.</p>
            </div>
        </div>
    </section>
    <section id="contact" class="contact">
        <h2>Contato</h2>
        <form>
            <label for="name">Nome:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Mensagem:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>
    <footer class="footer">
        <p>&copy; 2024 Meu Portfólio. Todos os direitos reservados.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

.header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

.header h1 {
    margin: 0;
}

.header nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0 0;
}

.header nav ul li {
    display: inline;
    margin: 0 10px;
}

.header nav ul li a {
    color: #fff;
    text-decoration: none;
}

.about, .projects, .contact {
    padding: 50px 20px;
    text-align: center;
}

.projects-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.project-card {
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px;
    width: 200px;
    text-align: center;
}

.project-card img {
    max-width: 100%;
    height: auto;
    border-radius: 5px;
}

.contact form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.contact form input, .contact form textarea {
    width: 100%;
    max-width: 500px;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
}

.contact form button {
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    background-color: #333;
    color: #fff;
    cursor: pointer;
}

.contact form button:hover {
    background-color: #555;
}

.footer {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}
document.addEventListener('DOMContentLoaded', () => {
    const form = document.querySelector('form');

    form.addEventListener('submit', (e) => {
        e.preventDefault();
        alert('Formulário enviado com sucesso!');
    });
});
