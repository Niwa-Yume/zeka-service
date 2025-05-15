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

  <section id="who-we-are" class="who-we-are">
    <div class="container">
      <h2>Qui sommes-nous&nbsp;?</h2>
      <p>
        Zeka Services Sàrl est une entreprise familiale suisse fondée en 2010.
        Nous proposons des services d’aménagement extérieur, de rénovation intérieur
        et de déménagement, alliant expertise, proximité et qualité.
      </p>
    </div>
  </section>

  <section id="services" class="services-modern">
    <div class="container">
      <h2>Nos Services</h2>
      <div class="services-grid">
        <div class="service-item item-1">
          <div class="service-icon">
            <!-- SVG Carrelage -->
          </div>
          <h3>Carrelage</h3>
          <p>Sols techniques pour zones industrielles.</p>
        </div>
        <div class="service-item item-2">
          <div class="service-icon">
            <!-- SVG Peinture -->
          </div>
          <h3>Peinture</h3>
          <p>Revêtements anti-corrosion sur mesure.</p>
        </div>
        <div class="service-item item-3">
          <div class="service-icon">
            <!-- SVG Aménagement Extérieur -->
          </div>
          <h3>Extérieur</h3>
          <p>Espaces sécurisés et esthétiques.</p>
        </div>
        <div class="service-item item-4">
          <div class="service-icon">
            <!-- SVG Déménagement -->
          </div>
          <h3>Déménagement</h3>
          <p>Logistique sans interruption.</p>
        </div>
        <div class="service-item item-5">
          <div class="service-icon">
            <!-- SVG Électricité -->
          </div>
          <h3>Électricité</h3>
          <p>Installations certifiées 24/7.</p>
        </div>
        <div class="service-item item-6">
          <div class="service-icon">
            <!-- SVG Plomberie -->
          </div>
          <h3>Plomberie</h3>
          <p>Dépannage et maintenance rapide.</p>
        </div>
      </div>
      <div class="services-cta">
        <button class="btn-primary">Découvrir tous les services</button>
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

  <section id="contact" class="contact">
    <div class="container">
      <h2 class="contact-title">Restons en contact</h2>
      <p class="contact-intro">
        Une question, un projet ou simplement envie d’échanger ?
        Notre équipe familiale est à votre écoute.
      </p>
      <div class="contact-grid">
        <div class="contact-details">
          <div class="info-item">
            <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
              <path d="M12 2C8.1 2 5 5.1 5 9c0 5.2 7 13 7 13s7-7.8 7-13c0-3.9-3.1-7-7-7zm0 9.5c-1.4 0-2.5-1.1-2.5-2.5S10.6 6.5 12 6.5s2.5 1.1 2.5 2.5S13.4 11.5 12 11.5z"/>
            </svg>
            <p><strong>Adresse</strong><br>CH-1006 Lausanne</p>
          </div>
          <div class="info-item">
            <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
              <path d="M6.6 10.8l2.2-2.2c.3-.3.7-.4 1.1-.3 1.2.3 2.4 1 3.5 2.1 1.1 1.1 1.8 2.3 2.1 3.5.1.4 0 .8-.3 1.1l-2.2 2.2c-.4.4-1 .5-1.5.3-1.7-.6-3.5-2.4-4.1-4.1-.2-.5-.1-1.1.3-1.5z"/>
            </svg>
            <p>
              <strong>Téléphone</strong><br>
              <a href="tel:+41797898848">+41 79 789 88 48</a>
            </p>
          </div>
          <div class="info-item">
            <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
              <path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
            </svg>
            <p>
              <strong>Email</strong><br>
              <a href="mailto:info@zeka-service.ch">info@zeka-service.ch</a>
            </p>
          </div>
        </div>
        <form class="contact-form" novalidate>
          <h3 class="form-title">Envoyez-nous un message</h3>
          <label>
            Prénom et nom*
            <input type="text" required aria-required="true" />
          </label>
          <label>
            E-mail*
            <input type="email" required aria-required="true" />
          </label>
          <label>
            Téléphone
            <input type="tel" />
          </label>
          <label>
            Message*
            <textarea rows="4" required aria-required="true"></textarea>
          </label>
          <button type="submit" class="btn-primary btn-contact">Envoyer</button>
        </form>
      </div>
    </div>
  </section>

  <footer id="footer" class="footer-enhanced">
    <div class="container">
      <h2 class="footer-title">Construisons l’avenir ensemble</h2>
      <p class="footer-intro">
        ZEKA Services, c’est la promesse d’un accompagnement sur-mesure, basé sur la confiance, l’expertise et la proximité.
      </p>
      <div class="footer-content">
        <div class="footer-item">
          <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
            <path d="M12 2L2 7l10 5 10-5-10-5zm0 7l-10 5 10 5 10-5-10-5z"/>
          </svg>
          <h3 class="footer-subtitle">Nos valeurs</h3>
          <p>Confiance, Qualité, Proximité</p>
        </div>
        <div class="footer-item">
          <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
            <path d="M3 3h18v4H3V3zm0 6h18v12H3V9z"/>
          </svg>
          <h3 class="footer-subtitle">Notre mission</h3>
          <p>Transformer vos espaces avec passion et professionnalisme.</p>
        </div>
        <div class="footer-item">
          <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
            <path d="M12 12c2.7 0 5-2.3 5-5s-2.3-5-5-5-5 2.3-5 5 2.3 5 5 5zm0 2c-3.3 0-10 1.7-10 5v3h20v-3c0-3.3-6.7-5-10-5z"/>
          </svg>
          <h3 class="footer-subtitle">Notre équipe</h3>
          <p>Une famille passionnée, à votre service depuis 2010.</p>
        </div>
      </div>
      <div class="footer-cta">
        <a href="#contact" class="btn-secondary">Contactez-nous</a>
      </div>
      <p class="footer-copy">© 2024 ZEKA Services Sàrl — Tous droits réservés</p>
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
.header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nav {
  display: flex;
  gap: 2rem;
}
.nav a {
  padding: 0.5rem 1rem;
  border-radius: 4px;
  color: var(--white);
  text-decoration: none;
  font-weight: 500;
  transition: background 0.3s, color 0.3s;
}
.nav a:hover {
  background: rgba(244, 197, 66, 0.1);
  color: var(--teal);
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

/* Section Who We Are */
.who-we-are {
  padding: 4rem 1rem;
  background: var(--white);
}
.who-we-are h2 {
  text-align: center;
  font-size: 2.5rem;
  color: var(--teal);
  margin-bottom: 1rem;
}
.who-we-are p {
  max-width: 700px;
  margin: 0 auto;
  text-align: center;
  font-size: 1.1rem;
  line-height: 1.6;
  color: var(--text);
}


/* Section Services */
.services-modern {
  padding: 4rem 1rem;
  background: var(--light);
}

.services-modern h2 {
  text-align: center;
  color: var(--teal);
  font-size: 2.5rem;
  margin-bottom: 2rem;
}

.services-grid {
  display: grid;
  grid-template-columns: 2fr 1fr 1fr;
  grid-template-rows: auto auto auto;
  grid-template-areas:
    "a a b"
    "a a c"
    "d e f";
  gap: 1.5rem;
}

.item-1 { grid-area: a; }
.item-2 { grid-area: b; }
.item-3 { grid-area: c; }
.item-4 { grid-area: d; }
.item-5 { grid-area: e; }
.item-6 { grid-area: f; }

.service-item {
  background: var(--white);
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  transition: transform 0.3s, box-shadow 0.3s;
}

.service-item:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 20px rgba(0,0,0,0.15);
}

.service-icon {
  width: 3rem;
  height: 3rem;
  margin-bottom: 1rem;
  fill: var(--yellow);
}

.services-cta {
  text-align: center;
  margin-top: 2.5rem;
}

.btn-primary {
  background: var(--yellow);
  color: var(--teal);
  padding: 0.75rem 2rem;
  border: none;
  border-radius: 4px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.3s;
}

.btn-primary:hover {
  background: #e5b731;
}


/* Section À propos */
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
  content: "\2713";
  position: absolute;
  left: 0;
  color: var(--yellow);
}
.about-cta {
  text-align: center;
  margin-top: 3rem;
}

/* Section Contact */
/* Section Contact */
.contact {
  padding: 4rem 1rem;
  background: var(--white);
}

.contact-title {
  font-size: 2.5rem;
  color: var(--teal);
  text-align: center;
  margin-bottom: 1rem;
}

.contact-intro {
  max-width: 600px;
  margin: 0 auto 2rem;
  text-align: center;
  color: var(--text);
  font-size: 1.1rem;
  line-height: 1.5;
}

/* Layout responsive */
.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

/* Bloc informations */
.contact-details .info-item {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.info-item .icon {
  width: 2.5rem;
  height: 2.5rem;
  fill: var(--teal);
}

.contact-details p {
  margin: 0;
  color: var(--text);
  font-size: 0.95rem;
}

/* Formulaire */
.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.form-title {
  font-size: 1.8rem;
  color: var(--teal);
  margin-bottom: 0.5rem;
}

.contact-form label {
  display: flex;
  flex-direction: column;
  font-size: 0.9rem;
  color: var(--text);
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-family: inherit;
}

/* Bouton d’envoi */
.btn-contact {
  width: fit-content;
  background: var(--teal);
  color: var(--white);
  padding: 0.75rem 2rem;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: background 0.3s;
}

.btn-contact:hover {
  background: #264f56;
}

/* Footer Enhanced */
.footer-enhanced {
  background: var(--teal);
  color: var(--white);
  padding: 3rem 1rem;
}
.footer-title {
  font-size: 2rem;
  font-weight: 700;
  text-align: center;
  color: var(--yellow);
}
.footer-intro {
  max-width: 600px;
  margin: 0.5rem auto 2rem;
  font-size: 1rem;
  text-align: center;
  line-height: 1.5;
}
.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
  margin-bottom: 2rem;
}
.footer-item {
  text-align: center;
}
.footer-item .icon {
  width: 2rem;
  height: 2rem;
  fill: var(--yellow);
  margin-bottom: 0.5rem;
}
.footer-subtitle {
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
}
.footer-cta {
  text-align: center;
  margin-bottom: 1.5rem;
}
.btn-secondary {
  display: inline-block;
  padding: 0.75rem 2rem;
  border: 2px solid var(--yellow);
  border-radius: 4px;
  color: var(--yellow);
  font-weight: 600;
  transition: background 0.3s, color 0.3s;
}
.btn-secondary:hover {
  background: var(--yellow);
  color: var(--teal);
}
.footer-copy {
  font-size: 0.85rem;
  text-align: center;
  opacity: 0.8;
}

/* Responsive */
@media (max-width: 768px) {
  .services-enhanced {
    padding: 3rem 1rem;
  }
  .about-title {
    font-size: 2rem;
  }
  .about-intro {
    font-size: 1rem;
  }
  .about-grid,
  .footer-content,
  .contact-grid {
    grid-template-columns: 1fr;
  }
  .services-grid {
    grid-template-columns: 1fr;
    grid-template-areas: none;
  }
  .contact-grid {
    grid-template-columns: 1fr;
  }
  .service-item {
    width: 100%;
  }
  .who-we-are {
    padding: 3rem 1rem;
  }
  .who-we-are h2 {
    font-size: 2rem;
  }
  .who-we-are p {
    font-size: 1rem;
  }
}
</style>