<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#090909">
<meta name="description" content="DY MEDIA – Dancun Yegon Creative Studios. Professional photography, videography, live streaming and website design. Capturing Moments. Creating Stories.">
<title>DY MEDIA | Dancun Yegon Creative Studios</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">

<style>
:root {
  --gold: #c9a45c;
  --gold-light: #e5c98d;
  --black: #090909;
  --dark: #111111;
  --card: #171717;
  --white: #ffffff;
  --muted: #aaa49a;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  font-family: 'DM Sans', sans-serif;
  background: var(--black);
  color: var(--white);
  line-height: 1.7;
}

a { text-decoration: none; color: inherit; }
img { width: 100%; display: block; }
button { font: inherit; }

.container {
  width: min(1160px, 90%);
  margin: auto;
}

.gold { color: var(--gold); }

.section {
  padding: 100px 0;
}

.section-heading {
  max-width: 680px;
  margin-bottom: 45px;
}

.section-heading .eyebrow {
  color: var(--gold);
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 4px;
  text-transform: uppercase;
}

.section-heading h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(32px, 5vw, 49px);
  line-height: 1.2;
  margin: 12px 0;
}

.section-heading p {
  color: var(--muted);
}

/* NAVIGATION */

header {
  position: fixed;
  z-index: 1000;
  top: 0;
  width: 100%;
  background: rgba(9,9,9,.94);
  border-bottom: 1px solid rgba(201,164,92,.18);
  backdrop-filter: blur(15px);
}

nav {
  height: 82px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 25px;
  font-weight: 800;
  letter-spacing: 2px;
}

.logo span { color: var(--gold); }

.logo small {
  display: block;
  font-size: 9px;
  color: var(--muted);
  letter-spacing: 3px;
  font-weight: 500;
  line-height: 1;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 28px;
  list-style: none;
}

.nav-links a {
  font-size: 13px;
  color: #ddd;
  transition: .3s;
}

.nav-links a:hover { color: var(--gold); }

.nav-contact {
  border: 1px solid var(--gold) !important;
  padding: 10px 18px;
  color: var(--gold) !important;
}

.menu-toggle {
  display: none;
  border: 0;
  background: none;
  color: white;
  font-size: 27px;
  cursor: pointer;
}

/* HERO */

.hero {
  min-height: 780px;
  height: 100vh;
  max-height: 950px;
  display: flex;
  align-items: center;
  position: relative;
  background:
    linear-gradient(90deg, rgba(0,0,0,.91), rgba(0,0,0,.52), rgba(0,0,0,.22)),
    linear-gradient(0deg, rgba(0,0,0,.55), transparent),
    url('https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?auto=format&fit=crop&w=2000&q=90') center/cover;
}

.hero-content {
  padding-top: 75px;
  max-width: 760px;
}

.hero-label {
  color: var(--gold-light);
  letter-spacing: 5px;
  font-size: 12px;
  font-weight: 700;
  text-transform: uppercase;
}

.hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(47px, 7vw, 82px);
  line-height: 1.12;
  margin: 23px 0;
}

.hero h1 span { color: var(--gold); }

.hero p {
  color: #d4d4d4;
  max-width: 560px;
  font-size: 17px;
  margin-bottom: 34px;
}

.buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 14px 25px;
  font-weight: 700;
  font-size: 13px;
  transition: .3s;
  cursor: pointer;
}

.btn-gold {
  background: var(--gold);
  color: #111;
}

.btn-gold:hover {
  background: var(--gold-light);
  transform: translateY(-3px);
}

.btn-outline {
  border: 1px solid rgba(255,255,255,.7);
  color: white;
}

.btn-outline:hover {
  border-color: var(--gold);
  color: var(--gold);
}

.hero-bottom {
  position: absolute;
  bottom: 35px;
  left: 5%;
  right: 5%;
  display: flex;
  justify-content: space-between;
  color: #ddd;
  font-size: 11px;
  letter-spacing: 2px;
}

/* INTRO */

.intro {
  background: #101010;
  border-top: 1px solid #242424;
  border-bottom: 1px solid #242424;
  padding: 32px 0;
}

.intro-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 25px;
  flex-wrap: wrap;
}

.intro-item {
  font-size: 12px;
  letter-spacing: 2px;
  color: #d5d0c7;
  font-weight: 600;
}

/* ABOUT */

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 65px;
  align-items: center;
}

.about-image {
  position: relative;
}

.about-image img {
  height: 510px;
  object-fit: cover;
}

.image-label {
  position: absolute;
  bottom: -20px;
  right: -20px;
  padding: 20px 25px;
  background: var(--gold);
  color: #111;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 2px;
}

.about-text h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(34px, 4vw, 48px);
  line-height: 1.2;
  margin: 15px 0 25px;
}

.about-text p {
  color: var(--muted);
  margin-bottom: 18px;
}

.signature {
  color: var(--gold);
  font-family: 'Playfair Display', serif;
  font-size: 25px;
  margin-top: 25px;
}

/* SERVICES */

.services {
  background: #101010;
}

.service-grid {
  display: grid;
  grid-template-columns: repeat(4,1fr);
  gap: 18px;
}

.service-card {
  padding: 32px 24px;
  background: var(--card);
  border: 1px solid #292929;
  transition: .35s;
}

.service-card:hover {
  border-color: var(--gold);
  transform: translateY(-7px);
  background: #1d1b17;
}

.service-number {
  font-size: 12px;
  color: var(--gold);
  letter-spacing: 2px;
}

.service-icon {
  font-size: 34px;
  margin: 22px 0;
}

.service-card h3 {
  font-family: 'Playfair Display', serif;
  font-size: 22px;
  margin-bottom: 12px;
}

.service-card p {
  color: var(--muted);
  font-size: 13px;
}

/* PORTFOLIO */

.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 18px;
}

.portfolio-item {
  position: relative;
  overflow: hidden;
  background: #171717;
  cursor: pointer;
  min-height: 300px;
}

.portfolio-item img {
  height: 330px;
  object-fit: cover;
  transition: .6s;
}

.portfolio-item:hover img {
  transform: scale(1.08);
}

.portfolio-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(0deg, rgba(0,0,0,.9), transparent 65%);
  display: flex;
  align-items: flex-end;
  padding: 25px;
}

.portfolio-overlay h3 {
  font-family: 'Playfair Display', serif;
  font-size: 23px;
}

.portfolio-overlay p {
  font-size: 12px;
  color: var(--gold-light);
}

/* QUOTE */

.quote-section {
  background: linear-gradient(rgba(0,0,0,.8),rgba(0,0,0,.88)),
  url('https://images.unsplash.com/photo-1516035069371-29a1b244cc32?auto=format&fit=crop&w=1800&q=85') center/cover fixed;
  text-align: center;
  padding: 110px 20px;
}

.quote-section h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(34px,5vw,55px);
  max-width: 850px;
  margin: auto;
  line-height: 1.3;
}

.quote-section p {
  color: var(--gold);
  letter-spacing: 4px;
  margin-top: 25px;
  font-size: 12px;
}

/* PROCESS */

.process-grid {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 30px;
}

.process-card {
  border-left: 2px solid var(--gold);
  padding: 8px 0 8px 24px;
}

.process-card span {
  color: var(--gold);
  font-size: 12px;
  letter-spacing: 3px;
}

.process-card h3 {
  font-family: 'Playfair Display', serif;
  margin: 12px 0;
  font-size: 22px;
}

.process-card p {
  color: var(--muted);
  font-size: 14px;
}

/* SOCIAL */

.social-section {
  background: #101010;
  text-align: center;
}

.social-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 14px;
  margin-top: 35px;
}

.social-links a {
  border: 1px solid #39352d;
  padding: 13px 21px;
  color: #ddd;
  font-size: 13px;
  transition: .3s;
}

.social-links a:hover {
  background: var(--gold);
  color: #111;
  border-color: var(--gold);
}

/* CONTACT */

.contact-grid {
  display: grid;
  grid-template-columns: .9fr 1.1fr;
  gap: 60px;
}

.contact-info h2 {
  font-family: 'Playfair Display', serif;
  font-size: 43px;
  line-height: 1.2;
  margin: 15px 0 20px;
}

.contact-info p {
  color: var(--muted);
  margin-bottom: 25px;
}

.contact-detail {
  padding: 16px 0;
  border-bottom: 1px solid #292929;
}

.contact-detail small {
  display: block;
  color: var(--gold);
  letter-spacing: 2px;
  font-size: 10px;
  margin-bottom: 5px;
}

.contact-detail a, .contact-detail span {
  font-size: 15px;
  color: #eee;
  overflow-wrap: anywhere;
}

.contact-form {
  background: var(--card);
  border: 1px solid #292929;
  padding: 35px;
}

.contact-form h3 {
  font-family: 'Playfair Display', serif;
  font-size: 27px;
  margin-bottom: 22px;
}

.contact-form label {
  display: block;
  color: #d7d0c3;
  font-size: 12px;
  margin: 14px 0 7px;
}

.contact-form input,
.contact-form select,
.contact-form textarea {
  width: 100%;
  background: #0d0d0d;
  color: white;
  border: 1px solid #393939;
  padding: 14px;
  outline: none;
  font-family: inherit;
  font-size: 14px;
}

.contact-form input:focus,
.contact-form select:focus,
.contact-form textarea:focus {
  border-color: var(--gold);
}

.contact-form textarea {
  resize: vertical;
  min-height: 120px;
}

.contact-form button {
  border: 0;
  width: 100%;
  margin-top: 20px;
}

/* FOOTER */

footer {
  background: #050505;
  border-top: 1px solid #28231b;
  padding: 55px 0 25px;
}

.footer-top {
  display: flex;
  justify-content: space-between;
  gap: 30px;
  flex-wrap: wrap;
  padding-bottom: 35px;
}

.footer-brand p {
  color: var(--muted);
  max-width: 330px;
  font-size: 13px;
  margin-top: 15px;
}

.footer-bottom {
  border-top: 1px solid #252525;
  padding-top: 22px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 15px;
  color: #8e8e8e;
  font-size: 11px;
}

/* WHATSAPP */

.whatsapp {
  position: fixed;
  right: 24px;
  bottom: 24px;
  z-index: 900;
  background: #20c66b;
  color: white;
  width: 58px;
  height: 58px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  font-size: 27px;
  box-shadow: 0 5px 25px rgba(0,0,0,.4);
  transition: .3s;
}

.whatsapp:hover { transform: scale(1.1); }

/* RESPONSIVE */

@media(max-width: 950px) {
  .service-grid { grid-template-columns: repeat(2,1fr); }
  .about-grid { gap: 35px; }
}

@media(max-width: 720px) {
  .section { padding: 75px 0; }
  nav { height: 70px; }
  .menu-toggle { display: block; }

  .nav-links {
    display: none;
    position: absolute;
    top: 70px;
    left: 0;
    width: 100%;
    padding: 25px 5%;
    background: #101010;
    flex-direction: column;
    align-items: flex-start;
    gap: 22px;
    border-bottom: 1px solid #333;
  }

  .nav-links.active { display: flex; }
  .hero { min-height: 700px; }
  .hero-bottom { font-size: 9px; }
  .about-grid, .contact-grid { grid-template-columns: 1fr; }
  .about-image img { height: 380px; }
  .image-label { right: 0; }
  .portfolio-grid { grid-template-columns: repeat(2,1fr); }
  .portfolio-item img { height: 250px; }
  .process-grid { grid-template-columns: 1fr; }
  .contact-grid { gap: 35px; }
}

@media(max-width: 440px) {
  .service-grid { grid-template-columns: 1fr; }
  .portfolio-grid { grid-template-columns: 1fr; }
  .portfolio-item img { height: 300px; }
  .hero h1 { font-size: 46px; }
  .contact-form { padding: 23px; }
  .intro-inner { justify-content: center; text-align: center; }
}
</style>
</head>

<body>

<header>
  <nav class="container">
    <a href="#home" class="logo">DY<span>MEDIA</span>
      <small>DANCUN YEGON CREATIVE STUDIOS</small>
    </a>

    <button class="menu-toggle" id="menuToggle" aria-label="Open navigation">☰</button>

    <ul class="nav-links" id="navLinks">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#social">Social Media</a></li>
      <li><a href="#contact" class="nav-contact">Contact Us</a></li>
    </ul>
  </nav>
</header>

<main>

<!-- HERO -->

<section class="hero" id="home">
  <div class="container">
    <div class="hero-content">
      <div class="hero-label">DANCUN YEGON CREATIVE STUDIOS</div>
      <h1>Capturing<br>Moments.<br><span>Creating Stories.</span></h1>
      <p>
        We bring ideas to life through professional photography,
        cinematic videography, live streaming and modern digital experiences.
      </p>
      <div class="buttons">
        <a href="#portfolio" class="btn btn-gold">EXPLORE OUR WORK</a>
        <a href="#contact" class="btn btn-outline">WORK WITH US</a>
      </div>
    </div>
  </div>

  <div class="hero-bottom">
    <span>CREATIVITY &nbsp; • &nbsp; QUALITY &nbsp; • &nbsp; EXCELLENCE</span>
    <span>DY MEDIA ©</span>
  </div>
</section>

<!-- INTRO STRIP -->

<section class="intro">
  <div class="container intro-inner">
    <div class="intro-item">PHOTOGRAPHY</div>
    <div class="intro-item">VIDEOGRAPHY</div>
    <div class="intro-item">LIVE STREAMING</div>
    <div class="intro-item">WEB DESIGN</div>
  </div>
</section>

<!-- ABOUT -->

<section class="section" id="about">
  <div class="container about-grid">
    <div class="about-image">
      <img src="https://images.unsplash.com/photo-1452587925148-ce544e77e70d?auto=format&fit=crop&w=1000&q=85" alt="Professional photography equipment">
      <div class="image-label">CREATIVE VISION</div>
    </div>

    <div class="about-text">
      <div class="hero-label">WHO WE ARE</div>
      <h2>Turning Your Vision Into <span class="gold">Visual Excellence.</span></h2>
      <p>
        DY MEDIA – Dancun Yegon Creative Studios is a creative media
        brand dedicated to capturing meaningful moments and transforming
        ideas into powerful visual experiences.
      </p>
      <p>
        From personal portraits and special events to professional video
        production, live broadcasts and websites, we combine creativity,
        technology and attention to detail to deliver memorable results.
      </p>
      <p>
        Every project deserves professionalism, passion and a unique story.
        We are here to help you tell yours.
      </p>
      <div class="signature">Dancun Yegon</div>
      <div class="gold">Founder & Creative Media Professional</div>
    </div>
  </div>
</section>

<!-- SERVICES -->

<section class="section services" id="services">
  <div class="container">
    <div class="section-heading">
      <div class="eyebrow">WHAT WE DO</div>
      <h2>Creative Services. <span class="gold">Professional Results.</span></h2>
      <p>Complete creative and digital solutions designed to make your brand, events and memories stand out.</p>
    </div>

    <div class="service-grid">

      <article class="service-card">
        <div class="service-number">01 / SERVICE</div>
        <div class="service-icon">📸</div>
        <h3>Photography</h3>
        <p>
          Portraits, events, personal branding, creative shoots
          and memorable moments captured with care.
        </p>
      </article>

      <article class="service-card">
        <div class="service-number">02 / SERVICE</div>
        <div class="service-icon">🎬</div>
        <h3>Videography</h3>
        <p>
          Professional video coverage, event films, promotional
          videos and cinematic storytelling.
        </p>
      </article>

      <article class="service-card">
        <div class="service-number">03 / SERVICE</div>
        <div class="service-icon">📡</div>
        <h3>Live Streaming</h3>
        <p>
          Professional live coverage for church services, conferences,
          events, interviews and special occasions.
        </p>
      </article>

      <article class="service-card">
        <div class="service-number">04 / SERVICE</div>
        <div class="service-icon">💻</div>
        <h3>Website Design</h3>
        <p>
          Modern, responsive websites for businesses, churches,
          organisations and personal brands.
        </p>
      </article>

    </div>
  </div>
</section>

<!-- PORTFOLIO -->

<section class="section" id="portfolio">
  <div class="container">
    <div class="section-heading">
      <div class="eyebrow">OUR CREATIVE WORLD</div>
      <h2>Selected <span class="gold">Visual Experiences.</span></h2>
      <p>A glimpse into the creative direction of DY MEDIA. Replace these sample photographs with your actual projects.</p>
    </div>

    <div class="portfolio-grid">

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=850&q=85" alt="Portrait photography">
        <div class="portfolio-overlay">
          <div><h3>Portraits</h3><p>PHOTOGRAPHY</p></div>
        </div>
      </div>

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=850&q=85" alt="Wedding event photography">
        <div class="portfolio-overlay">
          <div><h3>Special Events</h3><p>EVENT COVERAGE</p></div>
        </div>
      </div>

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1492619375914-88005aa9e8fb?auto=format&fit=crop&w=850&q=85" alt="Video production">
        <div class="portfolio-overlay">
          <div><h3>Film Production</h3><p>VIDEOGRAPHY</p></div>
        </div>
      </div>

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1470225620780-dba8ba36b745?auto=format&fit=crop&w=850&q=85" alt="Live event production">
        <div class="portfolio-overlay">
          <div><h3>Live Experiences</h3><p>LIVE STREAMING</p></div>
        </div>
      </div>

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=850&q=85" alt="Website development">
        <div class="portfolio-overlay">
          <div><h3>Digital Design</h3><p>WEB DESIGN</p></div>
        </div>
      </div>

      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=850&q=85" alt="Creative visual storytelling">
        <div class="portfolio-overlay">
          <div><h3>Creative Stories</h3><p>VISUAL STORYTELLING</p></div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- BRAND MESSAGE -->

<section class="quote-section">
  <h2>Every Picture Has a Story. Every Moment Deserves to Be Remembered.</h2>
  <p>DY MEDIA — CAPTURING MOMENTS. CREATING STORIES.</p>
</section>

<!-- PROCESS -->

<section class="section">
  <div class="container">
    <div class="section-heading">
      <div class="eyebrow">OUR APPROACH</div>
      <h2>From Your Idea to <span class="gold">The Final Creation.</span></h2>
      <p>We make the creative process simple, professional and collaborative.</p>
    </div>

    <div class="process-grid">
      <div class="process-card">
        <span>STEP 01</span>
        <h3>Let's Talk</h3>
        <p>Share your vision, event, project or creative idea with us.</p>
      </div>
      <div class="process-card">
        <span>STEP 02</span>
        <h3>We Create</h3>
        <p>We plan, produce and bring your project to life with creativity.</p>
      </div>
      <div class="process-card">
        <span>STEP 03</span>
        <h3>We Deliver</h3>
        <p>Receive a professional result designed to make an impression.</p>
      </div>
    </div>
  </div>
</section>

<!-- SOCIAL MEDIA -->

<section class="section social-section" id="social">
  <div class="container">
    <div class="section-heading" style="margin:0 auto;text-align:center">
      <div class="eyebrow">STAY CONNECTED</div>
      <h2>Follow Our <span class="gold">Creative Journey.</span></h2>
      <p>Connect with Dancun Yegon and discover our work, creativity and latest updates.</p>
    </div>

    <div class="social-links">
      <a href="https://www.tiktok.com/@dancuuh" target="_blank" rel="noopener">TikTok</a>
      <a href="https://www.youtube.com/@DYMEDIA-y8k" target="_blank" rel="noopener">YouTube</a>
      <a href="https://www.instagram.com/yegon3303?hvrq=Y253cWs1NmFzNG1o" target="_blank" rel="noopener">Instagram</a>
      <a href="https://t.me/dancuuh" target="_blank" rel="noopener">Telegram</a>
      <a href="https://x.com/dancuuh" target="_blank" rel="noopener">X / Twitter</a>
    </div>
  </div>
</section>

<!-- CONTACT -->

<section class="section" id="contact">
  <div class="container contact-grid">

    <div class="contact-info">
      <div class="eyebrow">LET'S CREATE SOMETHING GREAT</div>
      <h2>Have a Project in <span class="gold">Mind?</span></h2>
      <p>
        Whether you need photography, videography, live streaming
        or a professional website, we would love to hear from you.
        Let's discuss your next project.
      </p>

      <div class="contact-detail">
        <small>CALL / WHATSAPP</small>
        <a href="https://wa.me/254726684715" target="_blank" rel="noopener">0726684715</a>
      </div>

      <div class="contact-detail">
        <small>EMAIL ADDRESS</small>
        <a href="mailto:dancunyegon2000@gmail.com">dancunyegon2000@gmail.com</a>
      </div>

      <div class="contact-detail">
        <small>CREATIVE BRAND</small>
        <span>DY MEDIA – Dancun Yegon Creative Studios</span>
      </div>
    </div>

    <form class="contact-form" id="contactForm">
      <h3>Send Us an Enquiry</h3>

      <label for="name">Your Name</label>
      <input id="name" name="name" type="text" placeholder="Enter your name" required>

      <label for="phone">Your Phone Number</label>
      <input id="phone" name="phone" type="tel" placeholder="Enter your phone number" required>

      <label for="service">Service Required</label>
      <select id="service" name="service" required>
        <option value="">Select a service</option>
        <option>Photography</option>
        <option>Videography</option>
        <option>Live Streaming</option>
        <option>Website Design</option>
        <option>Other Enquiry</option>
      </select>

      <label for="message">Tell Us About Your Project</label>
      <textarea id="message" name="message" placeholder="Write your enquiry here..." required></textarea>

      <button class="btn btn-gold" type="submit">SEND ENQUIRY VIA WHATSAPP →</button>
    </form>

  </div>
</section>

</main>

<!-- FOOTER -->

<footer>
  <div class="container">
    <div class="footer-top">
      <div class="footer-brand">
        <a href="#home" class="logo">DY<span>MEDIA</span>
          <small>DANCUN YEGON CREATIVE STUDIOS</small>
        </a>
        <p>Professional photography, videography, live streaming and digital solutions. Capturing moments and creating stories that last.</p>
      </div>

      <div>
        <div class="gold">OUR SERVICES</div>
        <p>Photography</p>
        <p>Videography</p>
        <p>Live Streaming</p>
        <p>Website Design</p>
      </div>

      <div>
        <div class="gold">GET IN TOUCH</div>
        <p><a href="tel:0726684715">0726684715</a></p>
        <p><a href="mailto:dancunyegon2000@gmail.com">Email DY MEDIA</a></p>
        <p><a href="#contact">Start a Project</a></p>
      </div>
    </div>

    <div class="footer-bottom">
      <span>© <span id="year"></span> DY MEDIA. All Rights Reserved.</span>
      <span>CAPTURING MOMENTS. CREATING STORIES.</span>
    </div>
  </div>
</footer>

<!-- WHATSAPP FLOATING BUTTON -->

<a class="whatsapp"
   href="https://wa.me/254726684715?text=Hello%20DY%20MEDIA%2C%20I%20would%20like%20to%20make%20an%20enquiry."
   target="_blank"
   rel="noopener"
   aria-label="Contact DY MEDIA on WhatsApp">☏</a>

<script>
const menuToggle = document.getElementById('menuToggle');
const navLinks = document.getElementById('navLinks');

menuToggle.addEventListener('click', () => {
  navLinks.classList.toggle('active');
  menuToggle.textContent = navLinks.classList.contains('active') ? '✕' : '☰';
});

document.querySelectorAll('.nav-links a').forEach(link => {
  link.addEventListener('click', () => {
    navLinks.classList.remove('active');
    menuToggle.textContent = '☰';
  });
});

document.getElementById('year').textContent = new Date().getFullYear();

document.getElementById('contactForm').addEventListener('submit', function(event) {
  event.preventDefault();

  const name = document.getElementById('name').value.trim();
  const phone = document.getElementById('phone').value.trim();
  const service = document.getElementById('service').value;
  const message = document.getElementById('message').value.trim();

  if (!name || !phone || !service || !message) {
    alert('Please complete all fields.');
    return;
  }

  const text = `Hello DY MEDIA!

My name is ${name}.
My phone number is ${phone}.
Service required: ${service}.

Project details:
${message}

I would like to discuss this project with you.`;

  const whatsappURL = 'https://wa.me/254726684715?text=' + encodeURIComponent(text);
  window.open(whatsappURL, '_blank', 'noopener');
});
</script>

</body>
</html>
