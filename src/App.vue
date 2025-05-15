<script setup>
import logo from '@/assets/logo.jpg'

window.addEventListener('scroll', () => {
  const header = document.querySelector('.header');
  if (window.scrollY > 50) {
    header.classList.add('scrolled');
  } else {
    header.classList.remove('scrolled');
  }
});
</script>

<template>
  <header class="header">
    <div class="container">
      <img class="logo" :src="logo" alt="ZEKA Services">
      <nav class="nav">
        <a href="#accueil">Accueil</a>
        <a href="#about">À propos</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <section id="hero" class="hero">
    <div class="hero-content">
      <h1>ZEKA Services Sàrl</h1>
      <p>Aménagement extérieur<br>Rénovation intérieur | Déménagement</p>
      <button>CONTACTER</button>
    </div>
  </section>

  <section id="services" class="services">
    <h2>Nos services</h2>
    <div class="grid">
      <div class="card">
        <h3>Carrelage</h3>
        <p>Pour la pose de votre carrelage, faites appel à Zeka service, nous intervenons dans toute la Suisse.</p>
      </div>
      <div class="card">
        <h3>Déménagement</h3>
        <p>Zeka service prend en charge tous vos déménagements avec grand soin dans la Suisse.</p>
      </div>
      <div class="card">
        <h3>Entretien de jardin</h3>
        <p>Zeka service vous propose de tondre le gazon, tailler les arbustes, de l’arrosage…</p>
      </div>
      <div class="card">
        <h3>Maçonnerie</h3>
        <p>Pour tous vos travaux de maçonnerie, Zeka service met à votre service son savoir-faire.</p>
      </div>
      <div class="card">
        <h3>Montages des meubles</h3>
        <p>Montage et démontage de meubles. Avec Zeka Service, une solution rapide et efficace !</p>
      </div>
      <div class="card">
        <h3>Peinture</h3>
        <p>Zeka service vous fournit des services de peinture à l’intérieur et à l’extérieur.</p>
      </div>
    </div>
  </section>

  <section id="about" class="about">
    <div class="container">
      <h2 class="about-title">Notre ADN familial</h2>
      <p class="about-intro">
        Depuis 2010, <strong>ZEKA Services</strong> façonne vos espaces avec passion, savoir-faire et proximité.
      </p>

      <div class="about-grid">
        <div class="about-item">
          <i class="icon-mission"></i>
          <h3 class="about-subtitle">Notre mission</h3>
          <p class="about-text">
            Créer, innover et exécuter vos projets avec qualité et distinction.
          </p>
        </div>
        <div class="about-item">
          <i class="icon-history"></i>
          <h3 class="about-subtitle">Notre histoire</h3>
          <p class="about-text">
            Une entreprise familiale, une équipe dynamique et ouverte d’esprit à votre service.
          </p>
        </div>
        <div class="about-item">
          <i class="icon-vision"></i>
          <h3 class="about-subtitle">Notre vision</h3>
          <p class="about-text">
            Garantir un service optimal et une satisfaction client à 100 %.
          </p>
        </div>
        <div class="about-item">
          <i class="icon-values"></i>
          <h3 class="about-subtitle">Nos valeurs</h3>
          <ul class="about-values">
            <li>Confiance</li>
            <li>Qualité</li>
            <li>Proximité</li>
          </ul>
        </div>
      </div>

      <div class="about-cta">
        <button class="btn-primary">En savoir plus</button>
      </div>
    </div>
  </section>

  <section id="stats-contact" class="stats-contact">
    <div class="container">
      <div class="stats">
        <h2>Découvrez les quelques chiffres qui nous caractérisent</h2>
        <div class="grid">
          <div class="stat">
            <h3>2</h3>
            <p>collaborateurs</p>
          </div>
          <div class="stat">
            <h3>20</h3>
            <p>ans d'expérience</p>
          </div>
          <div class="stat">
            <h3>+ 500</h3>
            <p>projets terminés</p>
          </div>
          <div class="stat">
            <h3>2010</h3>
            <p>fondation</p>
          </div>
        </div>
      </div>

      <div class="contact-section">
        <h2>N’hésitez pas à nous contacter pour tout renseignement</h2>
        <div class="grid contact-grid">
          <div class="contact-form">
            <h3>Contact / Devis</h3>
            <form>
              <input type="text" placeholder="Prénom et nom*" required>
              <input type="email" placeholder="E-mail*" required>
              <input type="tel" placeholder="Téléphone*" required>
              <textarea placeholder="Message*" rows="4" required></textarea>
              <button type="submit">Envoyer</button>
            </form>
          </div>
          <div class="contact-info">
            <h3>Coordonnées</h3>
            <p><strong>Shefki Zeka</strong></p>
            <p>CH-1006 Lausanne</p>
            <p><a href="tel:+41797898848">+41 79 789 88 48</a></p>
            <p><a href="mailto:info@zeka-service.ch">info@zeka-service.ch</a></p>
            <p>Notre équipe est à votre disposition pour vous accompagner dans votre projet et répondre à toutes vos questions.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="container">
      <span>© 2024 ZEKA Services Sàrl</span>
      <nav class="nav">
        <a href="#accueil">Accueil</a>
        <a href="#about">À propos</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </footer>
</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  color: var(--text);
  background-color: var(--light);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

/* Header */
.header {
  position: fixed;
  top: 0;
  width: 100%;
  backdrop-filter: blur(10px);
  padding: 1rem 0;
  z-index: 1000;
  transition: background 0.3s ease-in-out;
}
.header.scrolled {
  background: rgba(46, 93, 103, 1);
}
.logo {
  height: 50px;
  border-radius: 50%;
  overflow: hidden;
}
.nav {
  display: flex;
  gap: 1.5rem;
}
.nav a {
  color: var(--white);
  text-decoration: none;
  font-weight: 500;
  font-size: 1rem;
  transition: color 0.3s ease;
}
.nav a:hover {
  color: var(--yellow);
}

/* Hero */
.hero {
  height: 80vh;
  background: url('https://source.unsplash.com/1600x900/?construction') center/cover;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}
.hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--teal);
  opacity: 0.6;
}
.hero-content {
  position: relative;
  text-align: center;
  color: var(--white);
  padding: 0 1rem;
}
.hero-content h1 {
  font-size: 3rem;
  font-weight: 700;
}
.hero-content p {
  margin: 1rem 0;
  font-size: 1.2rem;
  line-height: 1.5;
}
.hero-content button {
  background: var(--yellow);
  color: var(--teal);
  border: none;
  padding: 0.75rem 2rem;
  font-weight: 700;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.3s;
}
.hero-content button:hover {
  background: #e5b731;
}

/* Titres et grilles */
h2 {
  margin: 2rem 0 1rem;
  color: var(--teal);
  text-align: center;
}
.grid {
  display: grid;
  gap: 1rem;
}
.services .grid {
  grid-template-columns: 1fr;
}

/* Cartes */
.card {
  background: var(--white);
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
  text-align: center;
}

/* Section À propos améliorée */
.about {
  padding: 5rem 1rem;
  background: var(--light);
}
.about-title {
  font-size: 2.5rem;
  font-weight: 700;
  color: var(--teal);
  text-align: center;
  margin-bottom: 1rem;
}
.about-intro {
  max-width: 600px;
  margin: 0 auto 3rem;
  font-size: 1.2rem;
  text-align: center;
  color: var(--text);
}
.about-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 2rem;
}
.about-item {
  text-align: center;
}
.about-item i {
  font-size: 2rem;
  color: var(--yellow);
  margin-bottom: 0.5rem;
}
.about-subtitle {
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--teal);
  margin-bottom: 0.5rem;
}
.about-text {
  font-size: 1rem;
  line-height: 1.6;
  color: var(--text);
}
.about-values {
  list-style: none;
  padding: 0;
  margin: 1rem 0 0;
}
.about-values li {
  position: relative;
  padding-left: 1.5rem;
  margin-bottom: 0.5rem;
  color: var(--text);
}
.about-values li::before {
  content: "✔";
  position: absolute;
  left: 0;
  color: var(--yellow);
}
.about-cta {
  text-align: center;
  margin-top: 3rem;
}
.btn-primary {
  background: var(--yellow);
  color: var(--teal);
  padding: 0.75rem 2rem;
  font-weight: 600;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.3s;
}
.btn-primary:hover {
  background: #e5b731;
}

/* Stats et contact */
.stats-contact {
  padding: 4rem 1rem;
  background-color: var(--light);
}
.stats h2,
.contact-section h2 {
  text-align: center;
  color: var(--teal);
  margin-bottom: 2rem;
}
.stats .grid,
.contact-grid {
  display: grid;
  gap: 2rem;
}
.stats .grid {
  grid-template-columns: repeat(2, 1fr);
  text-align: center;
}
.stat h3 {
  font-size: 2.5rem;
  color: var(--yellow);
  margin-bottom: 0.5rem;
}
.stat p {
  font-size: 1rem;
  color: var(--text);
}
.contact-grid {
  grid-template-columns: 1fr 1fr;
  align-items: start;
}
.contact-form form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
.contact-form input,
.contact-form textarea {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 1rem;
}
.contact-form button {
  background: var(--yellow);
  color: var(--teal);
  padding: 0.75rem;
  border: none;
  font-weight: 700;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.3s;
}
.contact-form button:hover {
  background: #e5b731;
}
.contact-info p {
  margin: 0.5rem 0;
  color: var(--text);
}
.contact-info a {
  color: var(--teal);
  text-decoration: none;
}
.contact-info a:hover {
  text-decoration: underline;
}

/* Footer */
.footer {
  background: var(--teal);
  color: var(--white);
  padding: 1rem;
  text-align: center;
}

/* Responsive */
@media (max-width: 768px) {
  .services .grid {
    grid-template-columns: 1fr;
  }
  .about-title {
    font-size: 2rem;
  }
  .about-intro {
    font-size: 1rem;
  }
  .about-grid {
    grid-template-columns: 1fr;
  }
  .about-img {
    height: 200px;
  }
  .stats .grid,
  .contact-grid {
    grid-template-columns: 1fr;
  }
}
@media (min-width: 768px) {
  .services .grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>