<template>
  <div>
    <header class="header">
      <div class="container nav">
        <div class="logo">Tendance Hair</div>

        <nav>
          <a href="#salon">Le Salon</a>
          <a href="#prestations">Prestations</a>
          <a href="#equipe">Équipe</a>
          <a href="#contact">Contact</a>
        </nav>

        <a
          href="https://www.planity.com/tendance-hair-40500-saint-sever"
          target="_blank"
          class="btn"
        >
          Réserver
        </a>
      </div>
    </header>

    <section class="hero">
      <div class="overlay">
        <h1>Tendance Hair</h1>

        <p>
          Salon de coiffure à Saint-Sever spécialisé en coloration, balayage, coiffure mariage et
          conseils personnalisés.
        </p>

        <a
          href="https://www.planity.com/tendance-hair-40500-saint-sever"
          target="_blank"
          class="hero-btn"
        >
          Prendre rendez-vous
        </a>
      </div>
    </section>

    <section id="salon" class="section">
      <div class="container">
        <h2>Bienvenue chez Tendance Hair</h2>

        <p>
          Situé au cœur de Saint-Sever, notre salon vous accueille dans une ambiance chaleureuse et
          moderne.
        </p>

        <p>
          Notre équipe vous accompagne pour révéler votre style grâce à des techniques de coupe,
          coloration et soins capillaires adaptées à chaque personnalité.
        </p>
      </div>
    </section>

    <section id="prestations" class="section grey">
      <div class="container">
        <h2>Nos Prestations</h2>

        <div class="cards">
          <div class="card">
            <h3>Coupe Femme</h3>
            <p>Conseils personnalisés et tendances actuelles.</p>
          </div>

          <div class="card">
            <h3>Coupe Homme</h3>
            <p>Styles classiques ou modernes.</p>
          </div>

          <div class="card">
            <h3>Coloration</h3>
            <p>Couleurs éclatantes et techniques professionnelles.</p>
          </div>

          <div class="card">
            <h3>Balayage</h3>
            <p>Effets naturels et lumineux.</p>
          </div>

          <div class="card">
            <h3>Mariage</h3>
            <p>Coiffures élégantes pour le grand jour.</p>
          </div>

          <div class="card">
            <h3>Soins Capillaires</h3>
            <p>Nutrition et réparation du cheveu.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="gallery">
      <div class="container">
        <h2>Nos Réalisations</h2>

        <div class="gallery-grid">
          <img src="./gallery/1.jpg" alt="" />
          <img src="./gallery/2.jpg" alt="" />
          <img src="./gallery/3.jpg" alt="" />
          <img src="./gallery/4.jpg" alt="" />
          <img src="./gallery/5.jpg" alt="" />
        </div>
      </div>
    </section>

    <section id="equipe" class="section">
      <div class="container">
        <h2>Notre Équipe</h2>

        <div class="team">
          <div class="member">
            <h3>Daphné</h3>
            <p>Fondatrice & Experte Coloriste</p>
          </div>

          <div class="member">
            <h3>Cédrine</h3>
            <p>Coiffeuse Styliste</p>
          </div>

          <div class="member">
            <h3>Léo</h3>
            <p>Coiffeur Visagiste</p>
          </div>
        </div>
      </div>
    </section>

    <section class="cta">
      <div class="container">
        <h2>Envie d'un nouveau look ?</h2>

        <p>Réservez votre rendez-vous en quelques clics.</p>

        <a
          href="https://www.planity.com/tendance-hair-40500-saint-sever"
          target="_blank"
          class="hero-btn"
        >
          Réserver maintenant
        </a>
      </div>
    </section>

    <section id="contact" class="contact">
      <div class="container">
        <h2>Contact</h2>

        <div class="contact-grid">
          <div>
            <p><strong>Adresse</strong></p>
            <p>14 Rue du Général Lamarque</p>
            <p>40500 Saint-Sever</p>

            <br />

            <p><strong>Téléphone</strong></p>
            <p>05 58 76 33 76</p>
          </div>

          <iframe
            src="https://maps.google.com/maps?q=14%20Rue%20du%20General%20Lamarque%2040500%20Saint-Sever&t=&z=15&ie=UTF8&iwloc=&output=embed"
            loading="lazy"
          />
        </div>
      </div>
    </section>

    <footer>
      <p>© {{ new Date().getFullYear() }} Tendance Hair - Saint-Sever</p>
    </footer>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Poppins:wght@300;400;500;600&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Poppins, sans-serif;
  color: #222;
}

.container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}

.header {
  position: fixed;
  width: 100%;
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  z-index: 1000;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 80px;
}

.logo {
  font-family: Playfair Display;
  font-size: 28px;
  font-weight: bold;
}

nav {
  display: flex;
  gap: 30px;
}

nav a {
  text-decoration: none;
  color: #222;
}

.btn,
.hero-btn {
  background: #c79b5d;
  color: white;
  text-decoration: none;
  padding: 14px 28px;
  border-radius: 40px;
}

.hero {
  height: 100vh;
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/hero.jpg');
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.overlay {
  text-align: center;
  color: white;
  max-width: 800px;
}

.hero h1 {
  font-size: 72px;
  font-family: Playfair Display;
  margin-bottom: 20px;
}

.hero p {
  font-size: 20px;
  margin-bottom: 40px;
}

.section {
  padding: 100px 0;
}

.section h2 {
  text-align: center;
  margin-bottom: 40px;
  font-size: 42px;
  font-family: Playfair Display;
}

.grey {
  background: #f8f8f8;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
}

.card {
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
}

.gallery {
  padding: 100px 0;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.gallery-grid img {
  width: 100%;
  border-radius: 15px;
  height: 350px;
  object-fit: cover;
}

.team {
  display: flex;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
}

.member {
  text-align: center;
}

.cta {
  background: #111;
  color: white;
  text-align: center;
  padding: 120px 0;
}

.contact {
  padding: 100px 0;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
}

iframe {
  width: 100%;
  height: 400px;
  border: none;
  border-radius: 20px;
}

footer {
  background: #111;
  color: white;
  text-align: center;
  padding: 30px;
}

@media (max-width: 768px) {
  nav {
    display: none;
  }

  .hero h1 {
    font-size: 48px;
  }

  .gallery-grid {
    grid-template-columns: 1fr;
  }

  .contact-grid {
    grid-template-columns: 1fr;
  }

  .team {
    flex-direction: column;
  }
}
</style>
