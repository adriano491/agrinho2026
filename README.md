# agrinho2026
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AGRINHO 2026</title>

  <link rel="stylesheet" href="style.css">

  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
  />
</head>

<body>

  <!-- HEADER -->
  <header class="header">

    <div class="logo">
      <i class="fa-solid fa-leaf"></i>
      <h2>AGRINHO 2026</h2>
    </div>

    <nav class="navbar" id="navbar">
      <a href="#inicio">Início</a>
      <a href="#sobre">Sobre</a>
      <a href="#noticias">Notícias</a>
      <a href="#galeria">Galeria</a>
      <a href="#contato">Contato</a>
    </nav>

    <div class="header-buttons">

      <button id="darkModeToggle">
        <i class="fa-solid fa-moon"></i>
      </button>

      <button class="menu-btn" id="menuBtn">
        <i class="fa-solid fa-bars"></i>
      </button>

    </div>

  </header>

  <!-- HERO -->
  <section class="hero" id="inicio">

    <div class="hero-content">

      <h1>
        Recuperar o solo é cultivar o futuro
      </h1>

      <p>
        A recuperação de áreas degradadas fortalece a agricultura sustentável,
        protege o meio ambiente e garante alimento para as próximas gerações.
      </p>

      <a href="#noticias" class="hero-button">
        Explorar Notícias
      </a>

    </div>

  </section>

  <!-- SOBRE -->
  <section class="sobre" id="sobre">

    <div class="section-title">
      <h2>Sobre o Tema</h2>
      <p>
        Entenda a importância da recuperação ambiental para a agricultura.
      </p>
    </div>

    <div class="sobre-container">

      <div class="sobre-card">
        <i class="fa-solid fa-seedling"></i>
        <h3>Recuperação do Solo</h3>
        <p>
          Técnicas sustentáveis ajudam a restaurar áreas degradadas e aumentar
          a produtividade agrícola.
        </p>
      </div>

      <div class="sobre-card">
        <i class="fa-solid fa-tree"></i>
        <h3>Reflorestamento</h3>
        <p>
          O plantio de árvores auxilia na preservação da biodiversidade e do clima.
        </p>
      </div>

      <div class="sobre-card">
        <i class="fa-solid fa-water"></i>
        <h3>Uso Consciente da Água</h3>
        <p>
          Métodos inteligentes de irrigação reduzem desperdícios e preservam recursos.
        </p>
      </div>

    </div>

  </section>

  <!-- NOTÍCIAS -->
  <section class="noticias" id="noticias">

    <div class="section-title">
      <h2>Últimas Notícias</h2>
      <p>
        Informações sobre sustentabilidade e inovação agrícola.
      </p>
    </div>

    <div class="news-container" id="newsContainer">

      <!-- Notícias serão inseridas via JavaScript -->

    </div>

  </section>

  <!-- ESTATÍSTICAS -->
  <section class="estatisticas">

    <div class="stats-container">

      <div class="stat-card">
        <h2 class="counter" data-target="1500">0</h2>
        <p>Hectares Recuperados</p>
      </div>

      <div class="stat-card">
        <h2 class="counter" data-target="80">0</h2>
        <p>% Redução da Degradação</p>
      </div>

      <div class="stat-card">
        <h2 class="counter" data-target="300">0</h2>
        <p>Projetos Sustentáveis</p>
      </div>

      <div class="stat-card">
        <h2 class="counter" data-target="65">0</h2>
        <p>% Economia de Água</p>
      </div>

    </div>

  </section>

  <!-- GALERIA -->
  <section class="galeria" id="galeria">

    <div class="section-title">
      <h2>Galeria</h2>
      <p>
        Imagens inspiradoras sobre agricultura sustentável.
      </p>
    </div>

    <div class="galeria-container">

      <img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200&auto=format&fit=crop" alt="Agricultura">

      <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1200&auto=format&fit=crop" alt="Plantação">

      <img src="https://images.unsplash.com/photo-1472396961693-142e6e269027?q=80&w=1200&auto=format&fit=crop" alt="Natureza">

      <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?q=80&w=1200&auto=format&fit=crop" alt="Solo">

    </div>

  </section>

  <!-- CONTATO -->
  <section class="contato" id="contato">

    <div class="section-title">
      <h2>Contato</h2>
      <p>
        Entre em contato para saber mais sobre sustentabilidade agrícola.
      </p>
    </div>

    <form class="contact-form">

      <input type="text" placeholder="Seu Nome" required>

      <input type="email" placeholder="Seu Email" required>

      <textarea placeholder="Sua Mensagem" required></textarea>

      <button type="submit">
        Enviar Mensagem
      </button>

    </form>

  </section>

  <!-- FOOTER -->
  <footer class="footer">

    <h2>AGRINHO 2026</h2>

    <p>
      Recuperação de áreas degradadas para nova produção agrícola.
    </p>

    <div class="social-icons">

      <a href="#">
        <i class="fa-brands fa-instagram"></i>
      </a>

      <a href="#">
        <i class="fa-brands fa-facebook"></i>
      </a>

      <a href="#">
        <i class="fa-brands fa-youtube"></i>
      </a>

    </div>

    <p class="copy">
      © 2026 - Todos os direitos reservados.
    </p>

  </footer>

  <script src="script.js"></script>

</body>
</html>
