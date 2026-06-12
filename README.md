## index.html

```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Future Soil</title>

  <link rel="stylesheet" href="style.css">

  <link rel="preconnect" href="https://fonts.googleapis.com">

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap"
    rel="stylesheet">

  <link rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

</head>

<body>

  <!-- NAVBAR -->

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

    <button id="menu-btn">
      <i class="fa-solid fa-bars"></i>
    </button>

  </header>

  <!-- HERO -->

  <section class="hero" id="inicio">

    <img
      src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=1800&auto=format&fit=crop"
      class="hero-bg">

    <div class="overlay"></div>

    <div class="hero-content">

      <span class="hero-tag">
        Sustainability • Innovation • Future
      </span>

      <h1>
        Recuperar áreas degradadas é reconstruir o futuro
      </h1>

      <p>
        A tecnologia e a sustentabilidade trabalham juntas para transformar
        solos degradados em novas oportunidades para a agricultura moderna.
      </p>

      <a href="#sobre" class="hero-button">
        Explorar Projeto
      </a>

    </div>

  </section>

  <!-- SOBRE -->

  <section class="about" id="sobre">

    <div class="about-image">

      <img
        src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?q=80&w=1400&auto=format&fit=crop">

    </div>

    <div class="about-content">

      <span class="section-tag">
        SOBRE O PROJETO
      </span>

      <h2>
        Sustentabilidade conectada com inovação agrícola
      </h2>

      <p>
        Áreas degradadas afetam o meio ambiente, a biodiversidade
        e a produção agrícola. A recuperação do solo permite criar
        sistemas agrícolas mais eficientes, sustentáveis e preparados
        para o futuro.
      </p>

      <div class="glass-card">

        <i class="fa-solid fa-seedling"></i>

        <div>

          <h3>Recuperação Inteligente</h3>

          <p>
            Técnicas modernas ajudam a restaurar o equilíbrio natural do solo.
          </p>

        </div>

      </div>

    </div>

  </section>

  <!-- CARDS -->

  <section class="cards-section" id="impactos">

    <div class="section-center">

      <span class="section-tag">
        IMPACTOS POSITIVOS
      </span>

      <h2>
        Soluções sustentáveis para um novo futuro
      </h2>

    </div>

    <div class="cards-grid">

      <div class="card">

        <i class="fa-solid fa-tree"></i>

        <h3>Reflorestamento</h3>

        <p>
          Recuperação ambiental através da preservação da natureza.
        </p>

      </div>

      <div class="card">

        <i class="fa-solid fa-water"></i>

        <h3>Economia de Água</h3>

        <p>
          Irrigação inteligente reduz desperdícios e protege recursos.
        </p>

      </div>

      <div class="card">

        <i class="fa-solid fa-microchip"></i>

        <h3>Tecnologia</h3>

        <p>
          Sensores e inovação aumentam a produtividade sustentável.
        </p>

      </div>

    </div>

  </section>

  <!-- STATS -->

  <section class="stats">

    <div class="stat-box">

      <h2 class="counter" data-target="1200">0</h2>

      <p>Hectares Recuperados</p>

    </div>

    <div class="stat-box">

      <h2 class="counter" data-target="85">0</h2>

      <p>Redução da Degradação</p>

    </div>

    <div class="stat-box">

      <h2 class="counter" data-target="300">0</h2>

      <p>Projetos Sustentáveis</p>

    </div>

  </section>

  <!-- GALERIA -->

  <section class="gallery" id="galeria">

    <div class="section-center">

      <span class="section-tag">
        GALERIA
      </span>

      <h2>
        Natureza e inovação conectadas
      </h2>

    </div>

    <div class="gallery-grid">

      <img
        src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1200&auto=format&fit=crop">

      <img
        src="https://images.unsplash.com/photo-1492496913980-501348b61469?q=80&w=1200&auto=format&fit=crop">

      <img
        src="https://images.unsplash.com/photo-1523741543316-beb7fc7023d8?q=80&w=1200&auto=format&fit=crop">

      <img
        src="https://images.unsplash.com/photo-1472396961693-142e6e269027?q=80&w=1200&auto=format&fit=crop">

    </div>

  </section>

  <!-- FOOTER -->

  <footer class="footer">

    <h2>Future Soil</h2>

    <p>
      Innovation and sustainability for a better future.
    </p>

  </footer>

  <script src="script.js"></script>

</body>

</html>
```

---

## style.css

```css
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
  font-size:1.3rem;
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
  transition:.3s;
}

.navbar a:hover{
  color:#4ade80;
}

#menu-btn{
  display:none;
  background:none;
  border:none;
  color:white;
  font-size:1.5rem;
}

.hero{
  height:100vh;
  position:relative;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  overflow:hidden;
}

.hero-bg{
  position:absolute;
  width:100%;
  height:100%;
  object-fit:cover;
}

.overlay{
  position:absolute;
  width:100%;
  height:100%;
  background:rgba(0,0,0,0.6);
}

.hero-content{
  position:relative;
  z-index:2;
  max-width:900px;
  padding:20px;
}

.hero-tag{
  color:#4ade80;
  letter-spacing:2px;
}

.hero h1{
  font-size:5rem;
  margin:20px 0;
  line-height:1.1;
}

.hero p{
  font-size:1.1rem;
  color:#d1d5db;
  margin-bottom:40px;
}

.hero-button{
  padding:15px 40px;
  background:#4ade80;
  color:black;
  text-decoration:none;
  border-radius:50px;
  font-weight:600;
  transition:.3s;
}

.hero-button:hover{
  transform:translateY(-5px);
}

.about{
  padding:120px 8%;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:80px;
  align-items:center;
}

.about-image img{
  border-radius:25px;
}

.section-tag{
  color:#4ade80;
  letter-spacing:2px;
}

.about-content h2{
  font-size:3rem;
  margin:20px 0;
}

.about-content p{
  color:#cbd5e1;
  line-height:1.8;
}

.glass-card{
  margin-top:40px;
  padding:25px;
  border-radius:25px;
  background:rgba(255,255,255,0.05);
  backdrop-filter:blur(10px);
  display:flex;
  gap:20px;
  align-items:center;
}

.glass-card i{
  font-size:2rem;
  color:#4ade80;
}

.cards-section{
  padding:120px 8%;
}

.section-center{
  text-align:center;
  margin-bottom:70px;
}

.section-center h2{
  font-size:3rem;
  margin-top:15px;
}

.cards-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:30px;
}

.card{
  padding:40px;
  background:rgba(255,255,255,0.04);
  border:1px solid rgba(255,255,255,0.05);
  border-radius:25px;
  transition:.4s;
}

.card:hover{
  transform:translateY(-10px);
  background:rgba(255,255,255,0.08);
}

.card i{
  font-size:2rem;
  color:#4ade80;
  margin-bottom:20px;
}

.card h3{
  margin-bottom:15px;
}

.card p{
  color:#cbd5e1;
}

.stats{
  padding:120px 8%;
  display:flex;
  justify-content:center;
  gap:40px;
  flex-wrap:wrap;
}

.stat-box{
  text-align:center;
}

.stat-box h2{
  font-size:4rem;
  color:#4ade80;
}

.gallery{
  padding:120px 8%;
}

.gallery-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
  gap:20px;
}

.gallery-grid img{
  height:350px;
  object-fit:cover;
  border-radius:20px;
  transition:.4s;
}

.gallery-grid img:hover{
  transform:scale(1.03);
}

.footer{
  padding:60px 8%;
  text-align:center;
  border-top:1px solid rgba(255,255,255,0.08);
}

.footer p{
  margin-top:10px;
  color:#94a3b8;
}

@media(max-width:900px){

  .hero h1{
    font-size:3rem;
  }

  .about{
    grid-template-columns:1fr;
  }

  .navbar{
    display:none;
  }

  #menu-btn{
    display:block;
  }

}
```

---

## script.js

```javascript
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
```
