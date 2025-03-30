# trabalho-

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thomas Hobbes - Filosofia Política</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
            scroll-behavior: smooth; /* Animação suave ao rolar a página */
        }
        header {
            background: #0078d7;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }
        nav {
            background: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            transition: color 0.3s ease; /* Transição suave ao passar o mouse */
        }
        nav a:hover {
            color: #0078d7;
        }
        section {
            padding: 20px;
        }
        footer {
            background: #0078d7;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        /* Botão de voltar ao topo */
        #backToTop {
            position: fixed;
            bottom: 60px;
            right: 20px;
            background: #0078d7;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            display: none; /* Escondido por padrão */
            transition: opacity 0.3s ease;
        }
        #backToTop:hover {
            background: #005bb5;
        }
        /* Galeria de imagens */
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
        }
        .gallery img {
            width: 200px;
            height: 150px;
            object-fit: cover;
            border-radius: 5px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        /* Seção da equipe */
        .team {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .team-member {
            text-align: center;
            max-width: 200px;
        }
        .team-member img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Thomas Hobbes</h1>
        <p>O Filósofo do Contrato Social</p>
    </header>
    <nav>
        <a href="#sobre">Sobre</a>
        <a href="#filosofia">Filosofia</a>
        <a href="#galeria">Galeria</a>
        <a href="#equipe">Equipe</a>
        <a href="#contato">Contato</a>
    </nav>
    <section id="sobre">
        <h2>Sobre Thomas Hobbes</h2>
        <p>Thomas Hobbes (1588-1679) foi um filósofo inglês conhecido por sua obra "Leviatã", onde desenvolveu a teoria do contrato social. Ele acreditava que, para evitar o caos e a guerra, os indivíduos deveriam ceder parte de sua liberdade a um soberano absoluto, garantindo assim a paz e a ordem.</p>
    </section>
    <section id="filosofia">
        <h2>Filosofia de Hobbes</h2>
        <p>Hobbes defendia que, no estado de natureza, os homens viviam em constante conflito, em uma "guerra de todos contra todos". Para superar essa condição, era necessário estabelecer um contrato social, onde os indivíduos concordavam em submeter-se a um governo centralizado e absoluto.</p>
        <ul>
            <li><strong>Estado de Natureza:</strong> Uma condição de anarquia e insegurança.</li>
            <li><strong>Contrato Social:</strong> Um acordo entre os indivíduos para formar uma sociedade civil.</li>
            <li><strong>Leviatã:</strong> O soberano absoluto que garante a paz e a ordem.</li>
        </ul>
    </section>
    <section id="galeria">
        <h2>Galeria</h2>
        <div class="gallery">
            <a href="thomas-hobbes.webp" target="_blank">
                <img src="thomas-hobbes.webp" alt="Retrato de Hobbes">
            </a>
            <a href="https://fasbam.edu.br/wp-content/uploads/2020/06/Leviata%CC%83-Thomas-Hobbes.jpeg" target="_blank">
                <img src="" alt="Capa do Leviatã">
            </a>
            <a href="https://via.placeholder.com/200x150" target="_blank">
                <img src="https://via.placeholder.com/200x150" alt="Ilustração do Contrato Social">
            </a>
            <a href="https://via.placeholder.com/200x150" target="_blank">
                <img src="https://via.placeholder.com/200x150" alt="Representação do Estado de Natureza">
            </a>
        </div>
    </section>
    <section id="equipe">
        <h2>Equipe</h2>
        <div class="team">
            <div class="team-member">
                <img src="https://via.placeholder.com/100" alt="Membro 1">
                <h3>Kairon Arthur</h3>
                <p>Developer do site</p>
            </div>
            <div class="team-member">
                <img src="https://via.placeholder.com/100" alt="Membro 2">
                <h3>Maria Oliveira</h3>
                <p>Pesquisadora de Filosofia</p>
            </div>
            <div class="team-member">
                <img src="https://via.placeholder.com/100" alt="Membro 3">
                <h3>Ryan Soares</h3>
                <p>Co-orientador e historiador</p>
            </div>
        </div>
    </section>
    <section id="contato">
        <h2>Contato</h2>
        <p>Entre em contato conosco pelo e-mail: <a href="mailto:contato@siteinformativo.com" onclick="alert('Obrigado por entrar em contato!')">contato@siteinformativo.com</a></p>
        <button id="goToSite" onclick="redirectToSite()">Visite nosso parceiro</button>
    </section>
    <footer>
        <p>&copy; 2025 Thomas Hobbes - Filosofia Política. Todos os direitos reservados.</p>
    </footer>

    <!-- Botão de voltar ao topo -->
    <button id="backToTop" onclick="scrollToTop()">Topo</button>

    <script>
        // Mostrar o botão de "Voltar ao Topo" ao rolar a página
        window.onscroll = function() {
            const backToTopButton = document.getElementById('backToTop');
            if (document.documentElement.scrollTop > 100) {
                backToTopButton.style.display = 'block';
            } else {
                backToTopButton.style.display = 'none';
            }
        };

        // Função para rolar até o topo da página
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Função para redirecionar para outro site
        function redirectToSite() {
            window.location.href = "https://www.exemplo.com"; // Substitua pelo URL desejado
        }
    </script>
</body>
</html>
