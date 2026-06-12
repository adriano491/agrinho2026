<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Future Soil</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap"
    rel="stylesheet">

  <link rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins',sans-serif;
      background:#0b0f14;
      color:white;
      overflow-x:hidden;
    }

    img{
      width:100%;
      display:block;
    }

    section{
      width:100%;
    }

    /* HEADER */

    .header{
      width:100%;
      position:fixed;
      top:0;
      left:0;
      padding:25px 8%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      z-index:1000;
      background:rgba(0,0,0,0.2);
      backdrop-filter:blur(12px);
    }

    .logo{
      display:flex;
      align-items:center;
      gap:10px;
      font-size:1.4rem;
      font-weight:700;
    }

    .logo i{
      color:#4ade80;
    }

    .navbar{
      display:flex;
      gap:35px;
    }

    .navbar a{
      color:white;
      text-decoration:none;
      transition:0.3s;
      position:relative;
    }

    .navbar a::after{
      content:'';
      width:0%;
      height:2px;
      background:#4ade80;
      position:absolute;
      left:0;
      bottom:-5px;
      transition:0.3s;
    }

    .navbar a:hover::after{
      width:100%;
    }

    /* HERO */

    .hero{
      height:100vh;
      position:relative;
      display:flex;
      align-items:center;
      justify-content:center;
      overflow:hidden;
      text-align:center;
    }

    .hero video,
    .hero img{
      position:absolute;
      width:100%;
      height:100%;
      object-fit:cover;
    }

    .overlay{
      position:absolute;
      width:100%;
      height:100%;
      background:linear-gradient(to bottom,
      rgba(0,0,0,0.5),
      rgba(0,0,0,0.8));
    }

    .hero-content{
      position:relative;
      z-index:2;
      max-width:900px;
      padding:20px;
      animation:fadeUp 1.2s ease;
    }

    .hero-tag{
      color:#4ade80;
      letter-spacing:3px;
      font-size:0.9rem;
    }

    .hero h1{
      font-size:5rem;
      line-height:1.1;
      margin:20px 0;
    }

    .hero p{
      color:#d1d5db;
      font-size:1.2rem;
      line-height:1.8;
      margin-bottom:40px;
    }

    .hero-button{
      padding:18px 45px;
      border-radius:60px;
      background:#4ade80;
      color:black;
      text-decoration:none;
      font-weight:700;
      transition:0.4s;
      display:inline-block;
    }

    .hero-button:hover{
      transform:translateY(-6px);
      box-shadow:0 10px 30px rgba(74,222,128,0.3);
    }

    /* ABOUT */

    .about{
      padding:140px 8%;
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:80px;
      align-items:center;
    }

    .about-image{
      position:relative;
    }

    .about-image img{
      border-radius:30px;
      height:650px;
      object-fit:cover;
    }

    .floating-card{
      position:absolute;
      bottom:30px;
      right:-40px;
      background:rgba(255,255,255,0.08);
      backdrop-filter:blur(12px);
      padding:30px;
      border-radius:25px;
      width:280px;
      border:1px solid rgba(255,255,255,0.1);
    }

    .floating-card h3{
      color:#4ade80;
      margin-bottom:10px;
      font-size:2rem;
    }

    .section-tag{
      color:#4ade80;
      letter-spacing:3px;
      font-size:0.9rem;
    }

    .about-content h2{
      font-size:3.5rem;
      line-height:1.2;
      margin:20px 0;
    }

    .about-content p{
      color:#cbd5e1;
      line-height:2;
      margin-bottom:25px;
    }

    /* CARDS */

    .cards-section{
      padding:120px 8%;
    }

    .section-center{
      text-align:center;
      margin-bottom:70px;
    }

    .section-center h2{
      font-size:3rem;
      margin-top:20px;
    }

    .cards-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:30px;
    }

    .card{
      padding:40px;
      border-radius:30px;
      background:rgba(255,255,255,0.05);
      border:1px solid rgba(255,255,255,0.08);
      backdrop-filter:blur(12px);
      transition:0.4s;
      position:relative;
      overflow:hidden;
    }

    .card::before{
      content:'';
      position:absolute;
      width:200px;
      height:200px;
      background:rgba(74,222,128,0.08);
      border-radius:50%;
      top:-100px;
      right:-100px;
    }

    .card:hover{
      transform:translateY(-10px);
      background:rgba(255,255,255,0.08);
    }

    .card i{
      font-size:2.5rem;
      color:#4ade80;
      margin-bottom:25px;
    }

    .card h3{
      margin-bottom:15px;
      font-size:1.4rem;
    }

    .card p{
      color:#cbd5e1;
      line-height:1.8;
    }

    /* STATS */

    .stats{
      padding:140px 8%;
      background:
      linear-gradient(rgba(0,0,0,0.7),
      rgba(0,0,0,0.7)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1800&auto=format&fit=crop');
      background-size:cover;
      background-position:center;
      background-attachment:fixed;
    }

    .stats-container{
      display:flex;
      justify-content:center;
      gap:80px;
      flex-wrap:wrap;
      text-align:center;
    }

    .stat-box h2{
      font-size:5rem;
      color:#4ade80;
    }

    .stat-box p{
      color:#d1d5db;
      margin-top:10px;
    }

    /* GALLERY */

    .gallery{
      padding:140px 8%;
    }

    .gallery-grid{
      display:grid;
      grid-template-columns:repeat(4,1fr);
      grid-auto-rows:250px;
      gap:20px;
    }

    .gallery-item{
      overflow:hidden;
      border-radius:25px;
      position:relative;
    }

    .gallery-item img{
      height:100%;
      object-fit:cover;
      transition:0.5s;
    }

    .gallery-item:hover img{
      transform:scale(1.08);
    }

    .big{
      grid-column:span 2;
      grid-row:span 2;
    }

    /* FOOTER */

    .footer{
      padding:80px 8%;
      text-align:center;
      border-top:1px solid rgba(255,255,255,0.08);
    }

    .footer h2{
      font-size:2rem;
      margin-bottom:15px;
    }

    .footer p{
      color:#94a3b8;
    }

    /* ANIMATION */

    @keyframes fadeUp{

      from{
        opacity:0;
        transform:translateY(40px);
      }

      to{
        opacity:1;
        transform:translateY(0);
      }

    }

    /* RESPONSIVO */

    @media(max-width:1000px){

      .hero h1{
        font-size:3.5rem;
      }

      .about{
        grid-template-columns:1fr;
      }

      .about-image img{
        height:500px;
      }

      .floating-card{
        right:20px;
      }

      .gallery-grid{
        grid-template-columns:1fr 1fr;
      }

    }

    @media(max-width:700px){

      .navbar{
        display:none;
      }

      .hero h1{
        font-size:2.5rem;
      }

      .hero p{
        font-size:1rem;
      }

      .section-center h2,
      .about-content h2{
        font-size:2.2rem;
      }

      .gallery-grid{
        grid-template-columns:1fr;
      }

      .big{
        grid-column:auto;
        grid-row:auto;
      }

    }

  </style>

</head>

<body>

  <!-- HEADER -->

  <header class="header">

    <div class="logo">

      <i class="fa-solid fa-earth-americas"></i>

      <span>Future Soil</span>

    </div>

    <nav class="navbar">

      <a href="#inicio">Início</a>
      <a href="#sobre">Sobre</a>
      <a href="#impactos">Impactos</a>
      <a href="#galeria">Galeria</a>

    </nav>

  </header>

  <!-- HERO -->

  <section class="hero" id="inicio">

    <img
      src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1800&auto=format&fit=crop"
      alt="Natureza">

    <div class="overlay"></div>

    <div class="hero-content">

      <span class="hero-tag">
        SUSTAINABILITY • FUTURE • INNOVATION
      </span>

      <h1>
        Transformando áreas degradadas em novos futuros sustentáveis
      </h1>

      <p>
        Tecnologia, preservação ambiental e inovação agrícola trabalhando
        juntas para recuperar solos, proteger recursos naturais e criar
        uma agricultura mais inteligente para o futuro.
      </p>

      <a href="#sobre" class="hero-button">
        Explorar Projeto
      </a>

    </div>

  </section>

  <!-- ABOUT -->

  <section class="about" id="sobre">

    <div class="about-image">

      <img
        src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1400&auto=format&fit=crop"
        alt="Agricultura">

      <div class="floating-card">

        <h3>+1200</h3>

        <p>
          hectares recuperados através de soluções sustentáveis.
        </p>

      </div>

    </div>

    <div class="about-content">

      <span class="section-tag">
        SOBRE O PROJETO
      </span>

      <h2>
        Sustentabilidade conectada com inovação agrícola
      </h2>

      <p>
        O desgaste do solo afeta diretamente a agricultura, a biodiversidade
        e os recursos naturais. A recuperação ambiental permite devolver
        fertilidade à terra e criar sistemas agrícolas mais eficientes.
      </p>

      <p>
        Tecnologias sustentáveis ajudam a reduzir desperdícios, aumentar
        a produtividade e preservar o meio ambiente para as próximas gerações.
      </p>

    </div>

  </section>

  <!-- CARDS -->

  <section class="cards-section" id="impactos">

    <div class="section-center">

      <span class="section-tag">
        IMPACTOS POSITIVOS
      </span>

      <h2>
        Soluções sustentáveis para um planeta melhor
      </h2>

    </div>

    <div class="cards-grid">

      <div class="card">

        <i class="fa-solid fa-tree"></i>

        <h3>Reflorestamento</h3>

        <p>
          O plantio sustentável ajuda a recuperar áreas naturais e proteger a biodiversidade.
        </p>

      </div>

      <div class="card">

        <i class="fa-solid fa-water"></i>

        <h3>Economia de Água</h3>

        <p>
          Sistemas inteligentes reduzem desperdícios e preservam recursos hídricos.
        </p>

      </div>

      <div class="card">

        <i class="fa-solid fa-microchip"></i>

        <h3>Tecnologia Verde</h3>

        <p>
          Sensores e inovação ajudam a criar uma agricultura mais eficiente.
        </p>

      </div>

    </div>

  </section>

  <!-- STATS -->

  <section class="stats">

    <div class="stats-container">

      <div class="stat-box">

        <h2 class="counter" data-target="1200">0</h2>

        <p>
          hectares recuperados
        </p>

      </div>

      <div class="stat-box">

        <h2 class="counter" data-target="85">0</h2>

        <p>
          redução da degradação
        </p>

      </div>

      <div class="stat-box">

        <h2 class="counter" data-target="300">0</h2>

        <p>
          projetos sustentáveis
        </p>

      </div>

    </div>

  </section>

  <!-- GALLERY -->

  <section class="gallery" id="galeria">

    <div class="section-center">

      <span class="section-tag">
        VISUAL EXPERIENCE
      </span>

      <h2>
        Natureza, tecnologia e sustentabilidade
      </h2>

    </div>

    <div class="gallery-grid">

      <div class="gallery-item big">

        <img
          src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200&auto=format&fit=crop">

      </div>

      <div class="gallery-item">

        <img
          src="https://images.unsplash.com/photo-1492496913980-501348b61469?q=80&w=1200&auto=format&fit=crop">

      </div>

      <div class="gallery-item">

        <img
          src="https://images.unsplash.com/photo-1523741543316-beb7fc7023d8?q=80&w=1200&auto=format&fit=crop">

      </div>

      <div class="gallery-item">

        <img
          src="https://images.unsplash.com/photo-1472396961693-142e6e269027?q=80&w=1200&auto=format&fit=crop">

      </div>

    </div>

  </section>

  <!-- FOOTER -->

  <footer class="footer">

    <h2>Future Soil</h2>

    <p>
      Innovation and sustainability for a better future.
    </p>

  </footer>

  <script>

    const counters = document.querySelectorAll('.counter');

    counters.forEach(counter => {

      counter.innerText = '0';

      const updateCounter = () => {

        const target = +counter.getAttribute('data-target');
        const current = +counter.innerText;

        const increment = target / 100;

        if(current < target){

          counter.innerText = `${Math.ceil(current + increment)}`;

          setTimeout(updateCounter, 20);

        } else {

          counter.innerText = target;

        }

      };

      updateCounter();

    });

  </script>

</body>

</html>
