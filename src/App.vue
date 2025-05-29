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
    <div class="hero-glass">
      <div class="hero-content">
        <img class="hero-logo" :src="logo" alt="ZEKA Services">
        <h1>ZEKA Services Sàrl</h1>
        <p>Aménagement extérieur<br>Rénovation intérieur | Déménagement</p>
        <button>CONTACTER</button>
      </div>
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

  <section id="services" class="services">
    <div class="container">
      <h2 class="services-title">Nos Services</h2>
      <div class="services-grid">
        <div class="service-item item-1">
          <div class="service-overlay">
            <h3>Entretien de jardin</h3>
            <p>
              Entretien toute l’année: tonte de gazon, taille des arbustes, et tout ce qui concerne le jardin sur demande du client.
            </p>
          </div>
        </div>
        <div class="service-item item-2">
          <div class="service-overlay">
            <h3>Rénovation tous types d’intérieurs</h3>
            <p>
              Peinture, plâtrerie, démolition, façade, etc. sur demande.
            </p>
          </div>
        </div>
        <div class="service-item item-3">
          <div class="service-overlay">
            <h3>Aménagement Extérieur</h3>
            <p>
              Création de terrasses, terrassement, maçonnerie, entretien de jardin, plantation, abattage, tout type de clôtures et autres services.
            </p>
          </div>
        </div>
        <div class="service-item item-4">
          <div class="service-overlay">
            <h3>Déménagement</h3>
            <p>
              Tout type de déménagement partout en Suisse et à l’étranger (France, Belgique, Italie, autres pays selon demande).<br>
              Débarras, livraisons de tout type de marchandise, etc.
            </p>
          </div>
        </div>
        <div class="service-item item-5">
          <div class="service-overlay">
            <h3>Carrelage</h3>
            <p>Pose soignée de carreaux céramique, grès et marbre pour sols et murs, adaptés à chaque espace.</p>
          </div>
        </div>
        <div class="service-item item-6">
          <div class="service-overlay">
            <h3>Plomberie</h3>
            <p>Installation sanitaire, chauffage et détection de fuites, interventions rapides et garanties.</p>
          </div>
        </div>
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
              <path
                  d="M12 2C8.1 2 5 5.1 5 9c0 5.2 7 13 7 13s7-7.8 7-13c0-3.9-3.1-7-7-7zm0 9.5c-1.4 0-2.5-1.1-2.5-2.5S10.6 6.5 12 6.5s2.5 1.1 2.5 2.5S13.4 11.5 12 11.5z"/>
            </svg>
            <p><strong>Adresse</strong><br>CH-1006 Lausanne</p>
          </div>
          <div class="info-item">
            <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
              <path
                  d="M6.6 10.8l2.2-2.2c.3-.3.7-.4 1.1-.3 1.2.3 2.4 1 3.5 2.1 1.1 1.1 1.8 2.3 2.1 3.5.1.4 0 .8-.3 1.1l-2.2 2.2c-.4.4-1 .5-1.5.3-1.7-.6-3.5-2.4-4.1-4.1-.2-.5-.1-1.1.3-1.5z"/>
            </svg>
            <p>
              <strong>Téléphone</strong><br>
              <a href="tel:+41797898848">+41 79 789 88 48</a>
            </p>
          </div>
          <div class="info-item">
            <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
              <path
                  d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
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
            <input type="text" required aria-required="true"/>
          </label>
          <label>
            E-mail*
            <input type="email" required aria-required="true"/>
          </label>
          <label>
            Téléphone
            <input type="tel"/>
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

  <section id="instagram" class="instagram">
    <div class="container">
      <h2 class="instagram-title">Suivez-nous sur Instagram</h2>
      <p class="instagram-intro">Découvrez nos réalisations en temps réel</p>
      <div class="instagram-feed">
        <!-- Embed Instagram Feed -->
        <iframe
            class="instagram-embed"
            src="https://www.instagram.com/zekaservices.sarl/embed"
            frameborder="0"
            scrolling="no"
            allowtransparency="true">
        </iframe>
      </div>
      <div class="instagram-cta">
        <a href="https://www.instagram.com/zekaservices.sarl/" target="_blank" class="btn-secondary">
          @zekaservices.sarl
        </a>
      </div>
    </div>
  </section>

  <footer id="footer" class="footer-enhanced">
    <div class="container">
      <h2 class="footer-title">Construisons l’avenir ensemble</h2>
      <p class="footer-intro">
        ZEKA Services, c’est la promesse d’un accompagnement sur-mesure, basé sur la confiance, l’expertise et la
        proximité.
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
            <path
                d="M12 12c2.7 0 5-2.3 5-5s-2.3-5-5-5-5 2.3-5 5 2.3 5 5 5zm0 2c-3.3 0-10 1.7-10 5v3h20v-3c0-3.3-6.7-5-10-5z"/>
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
:root {
  --teal: #2E5D67;
  --yellow: #F4C542;
  --light: #F9F7F0;
  --text: #2A2A2A;
  --white: #FFFFFF;
}

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
/* Instagram Section */
.instagram {
  padding: 4rem 0;
  background: var(--light);
}

.instagram-title {
  text-align: center;
  font-size: 2.5rem;
  color: var(--teal);
  margin-bottom: 1rem;
}

.instagram-intro {
  text-align: center;
  margin-bottom: 2rem;
  color: var(--text);
  font-size: 1.1rem;
}

.instagram-feed {
  width: 100%;
  max-width: 800px;
  margin: 0 auto 2rem;
  aspect-ratio: 1;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  background: var(--white);
  position: relative;
}

.instagram-embed {
  width: 100%;
  height: 100%;
  border: none;
  display: block;
}

.instagram-cta {
  text-align: center;
  margin-top: 2rem;
}

.instagram-cta .btn-secondary {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: var(--white);
  padding: 0.75rem 2rem;
  border-radius: 4px;
  text-decoration: none;
  font-weight: 600;
  color: var(--teal);
  border: 2px solid var(--teal);
  transition: all 0.3s ease;
}

.instagram-cta .btn-secondary:hover {
  background: var(--teal);
  color: var(--white);
  transform: translateY(-2px);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
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
  display: block; /* Ajout pour garantir la visibilité */
}

.header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap; /* Permet le retour à la ligne sur mobile */
  gap: 1rem; /* Espace entre le logo et la navigation */
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
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  background:
      radial-gradient(ellipse at 60% 40%, rgba(244,197,66,0.25) 0%, transparent 60%),
      linear-gradient(120deg, #2E5D67 0%, #24C6DC 60%, #F4C542 100%);
  border-radius: 0 0 32px 32px;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.18);
  backdrop-filter: blur(18px) saturate(180%);
  -webkit-backdrop-filter: blur(18px) saturate(180%);
  overflow: hidden;
  margin-top: 40px;
}

.hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(255,255,255,0.10);
  z-index: 1;
  pointer-events: none;
  border-radius: 0 0 32px 32px;
  mix-blend-mode: lighten;
}

.hero-glass {
  position: relative;
  z-index: 2;
  background: rgba(255, 255, 255, 0.18);
  border-radius: 24px;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.18);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  padding: 3rem 2rem;
  max-width: 600px;
  width: 90%;
  margin: 0 auto;
  border: 1px solid rgba(255,255,255,0.25);
  display: flex;
  flex-direction: column;
  align-items: center;
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
.hero-logo {
  max-width: 320px;
  width: 90%;
  margin: 0 auto 2rem auto;
  display: block;
  background: transparent;
  filter: drop-shadow(0 2px 8px rgba(0,0,0,0.08));
}
/* Who We Are */
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

/* Services Section */
.services {
  padding: 4rem 0;
  background: var(--white);
}

.services .container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.services-title {
  text-align: center;
  font-size: 2.5rem;
  color: var(--teal);
  margin-bottom: 3rem;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  gap: 2rem;
  width: 100%;
}

.service-item {
  position: relative;
  border-radius: 12px;
  overflow: hidden;
  background-size: cover;
  background-position: center;
  min-height: 280px;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.service-item:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
}

.service-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(to top, rgba(0, 0, 0, 0.8) 0%, rgba(0, 0, 0, 0.3) 60%, rgba(0, 0, 0, 0.1) 100%);
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 2rem;
  color: #fff;
  transition: background 0.3s ease;
}

.service-item:hover .service-overlay {
  background: linear-gradient(to top, rgba(0, 0, 0, 0.9) 0%, rgba(0, 0, 0, 0.5) 60%, rgba(0, 0, 0, 0.2) 100%);
}

.service-overlay h3 {
  margin-bottom: 0.75rem;
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--yellow);
}

.service-overlay p {
  font-size: 1rem;
  line-height: 1.5;
  max-width: 100%;
}
.item-2,
.item-6 {
  grid-column: span 2;
}


.item-1 {
  background-image: url('@/assets/image-service/electricite.jpg');
  background-size: cover;
  background-position: center;
}
.item-3 {
  background-image: url('@/assets/image-service/carrelage.jpg');
  background-size: cover;
  background-position: center;
}
.item-4 {
  background-image: url('@/assets/image-service/demenagement.jpg');
  background-size: cover;
  background-position: center;
}
.item-6 {
  background-image: url('@/assets/image-service/plomberie.jpg');
  background-size: cover;
  background-position: center;
}
.item-5 {
  background-image: url('@/assets/image-service/chantier.jpg');
  background-size: cover;
  background-position: center;
}
.item-2 {
  background-image: url('@/assets/image-service/peinture.jpg');
  background-size: cover;
  background-position: center;
}

/* About Section */
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
  padding-right: 1.5rem;
  margin-bottom: 0.5rem;
  color: var(--text);
}

.about-values li::after {
  content: "\2713";
  position: absolute;
  padding-left: 2rem;
  color: var(--yellow);
}

.about-cta {
  text-align: center;
  margin-top: 3rem;
}

/* Contact Section */
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

.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  align-items: center;
}

.contact-details .info-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  background: var(--white);
  padding: 1rem;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  margin-bottom: 1rem;
  flex-direction: column;
  justify-content: center;
}

.info-item .icon {
  width: 2.5rem;
  height: 2.5rem;
  fill: var(--teal);
}

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

/* Footer */
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
.footer-cta{
  justify-content: center;
  display: flex;
  margin-bottom: 2rem;
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

.footer-copy {
  font-size: 0.85rem;
  text-align: center;
  opacity: 0.8;
}

/* Buttons */
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

/* Responsive */
@media (min-width: 576px) {
  .services-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 992px) {
  .services-grid {
    grid-template-columns: repeat(3, 1fr);
  }

  .item-1 {
    grid-column: span 1;
    grid-row: span 1;
  }

  .item-3 {
    grid-column: span 2;
  }
}

/* Media Queries */
@media (min-width: 576px) {
  .services-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 992px) {
  .services-grid {
    grid-template-columns: repeat(3, 1fr);
  }

  .item-1 {
    grid-column: span 1;
    grid-row: span 1;
  }

  .item-3 {
    grid-column: span 2;
  }
}

@media (min-width: 1200px) {
  .services-grid {
    gap: 2.5rem;
  }

  .service-overlay h3 {
    font-size: 1.75rem;
  }

  .service-overlay p {
    font-size: 1.1rem;
  }
}

@media (max-width: 768px) {
  .header .container {
    padding: 0 1rem;
  }

  .nav {
    display: flex !important;
    position: static;
    flex-direction: row;
    background: transparent;
    box-shadow: none;
    padding: 0;
    width: 100%;
    justify-content: center;
    gap: 0.5rem;
  }

  .nav a {
    padding: 0.5rem;
    font-size: 0.9rem;
  }

  .logo {
    height: 40px;
    margin:auto;
  }

  .about-grid,
  .contact-grid,
  .footer-content {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .nav {
    flex-wrap: wrap;
  }

  .nav a {
    font-size: 0.8rem;
    padding: 0.4rem;
  }

  .hero-content h1 {
    font-size: 2rem;
  }

  .hero-content p,
  .nav a {
    font-size: 0.9rem;
  }

  .services-grid {
    gap: 1.5rem;
  }

  .service-item {
    min-height: 220px;
  }

  .service-overlay {
    padding: 1.5rem;
  }

  .service-overlay h3 {
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
  }

  .service-overlay p {
    font-size: 0.9rem;
    line-height: 1.4;
  }
}

@media (max-width: 425px) {
  .service-item {
    min-height: 200px;
  }

  .service-overlay {
    padding: 1rem;
    background: rgba(0, 0, 0, 0.6);
  }
}
</style>