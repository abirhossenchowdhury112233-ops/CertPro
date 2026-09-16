# CertPro
CertPro - Professional Certification Preparation platfrom
index.html <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>CertPro | Certification Preparation</title>

  <meta name="description"
        content="CertPro provides certification preparation resources, practice materials and guidance.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      color: #111827;
      background: #ffffff;
      line-height: 1.6;
    }

    /* NAVBAR */

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(255,255,255,0.95);
      border-bottom: 1px solid #e5e7eb;
    }

    nav {
      max-width: 1200px;
      margin: auto;
      padding: 18px 25px;

      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 27px;
      font-weight: 800;
      color: #111827;
      text-decoration: none;
    }

    .logo span {
      color: #2563eb;
    }

    .menu {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    .menu a {
      text-decoration: none;
      color: #4b5563;
      font-weight: 600;
    }

    .menu a:hover {
      color: #2563eb;
    }

    .nav-btn {
      background: #2563eb;
      color: white;
      padding: 10px 17px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 700;
    }

    /* HERO */

    .hero {
      max-width: 1200px;
      margin: auto;
      min-height: 650px;
      padding: 90px 25px;

      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 60px;
      align-items: center;
    }

    .tag {
      color: #2563eb;
      font-weight: 800;
      font-size: 13px;
      letter-spacing: 2px;
      margin-bottom: 15px;
    }

    .hero h1 {
      font-size: clamp(45px, 6vw, 75px);
      line-height: 1.05;
      letter-spacing: -3px;
      margin-bottom: 25px;
    }

    .hero h1 span {
      color: #2563eb;
    }

    .hero p {
      color: #667085;
      font-size: 18px;
      max-width: 600px;
    }

    .buttons {
      margin-top: 30px;
      display: flex;
      gap: 12px;
    }

    .btn {
      padding: 14px 21px;
      border-radius: 9px;
      text-decoration: none;
      font-weight: 700;
      display: inline-block;
    }

    .primary {
      background: #2563eb;
      color: white;
    }

    .secondary {
      border: 1px solid #d1d5db;
      color: #111827;
    }

    /* HERO CARD */

    .hero-card {
      background: #111827;
      color: white;
      border-radius: 22px;
      padding: 35px;
      box-shadow: 0 25px 60px rgba(0,0,0,.15);
    }

    .hero-card small {
      color: #9ca3af;
      letter-spacing: 2px;
    }

    .hero-card h2 {
      font-size: 52px;
      margin: 15px 0 35px;
    }

    .item {
      border-top: 1px solid #374151;
      padding: 16px 0;

      display: flex;
      justify-content: space-between;
    }

    .item span {
      color: #60a5fa;
    }

    /* STATS */

    .stats {
      border-top: 1px solid #e5e7eb;
      border-bottom: 1px solid #e5e7eb;

      display: grid;
      grid-template-columns: repeat(3,1fr);
      text-align: center;
    }

    .stat {
      padding: 30px;
      border-right: 1px solid #e5e7eb;
    }

    .stat:last-child {
      border-right: none;
    }

    .stat strong {
      display: block;
      font-size: 30px;
    }

    .stat span {
      color: #667085;
    }

    /* SECTIONS */

    section.content {
      max-width: 1200px;
      margin: auto;
      padding: 100px 25px;
    }

    .section-title {
      margin-bottom: 45px;
    }

    .section-title h2 {
      font-size: 43px;
      letter-spacing: -1px;
    }

    .section-title p {
      color: #667085;
      margin-top: 10px;
    }

    /* CERTIFICATIONS */

    .cards {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 20px;
    }

    .card {
      padding: 30px;
      border: 1px solid #e5e7eb;
      border-radius: 15px;
      transition: .2s;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 15px 35px rgba(0,0,0,.07);
    }

    .icon {
      width: 50px;
      height: 50px;

      display: grid;
      place-items: center;

      background: #eff6ff;
      color: #2563eb;

      border-radius: 12px;
      font-weight: 900;

      margin-bottom: 20px;
    }

    .card h3 {
      margin-bottom: 8px;
    }

    .card p {
      color: #667085;
    }

    .card a {
      display: inline-block;
      margin-top: 18px;
      color: #2563eb;
      text-decoration: none;
      font-weight: 700;
    }

    /* SERVICES */

    .gray {
      background: #f8fafc;
    }

    .services {
      max-width: 1200px;
      margin: auto;
      padding: 100px 25px;
    }

    .service-grid {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 20px;
    }

    .service {
      background: white;
      padding: 32px;
      border-radius: 15px;
      border: 1px solid #e5e7eb;
    }

    .service-number {
      color: #2563eb;
      font-weight: 900;
    }

    .service h3 {
      margin: 15px 0 8px;
    }

    .service p {
      color: #667085;
    }

    /* CTA */

    .cta {
      max-width: 1150px;
      margin: 70px auto;
      padding: 65px 50px;

      border-radius: 22px;

      background: #111827;
      color: white;

      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 30px;
    }

    .cta p {
      color: #cbd5e1;
      margin-top: 10px;
    }

    /* CONTACT */

    .contact {
      max-width: 1200px;
      margin: auto;
      padding: 100px 25px;

      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 70px;
    }

    .contact-info p {
      margin: 12px 0;
      color: #667085;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 13px;
    }

    input,
    select,
    textarea {
      padding: 14px;
      border: 1px solid #d1d5db;
      border-radius: 9px;
      font-size: 15px;
      font-family: inherit;
    }

    textarea {
      resize: vertical;
    }

    button {
      border: none;
      cursor: pointer;
      font-size: 15px;
    }

    /* FOOTER */

    footer {
      border-top: 1px solid #e5e7eb;
      padding: 35px 25px;
      text-align: center;
    }

    footer p {
      color: #667085;
      margin-top: 8px;
      font-size: 13px;
    }

    /* MOBILE */

    @media(max-width:800px) {

      .menu {
        display: none;
      }

      .hero {
        grid-template-columns: 1fr;
        padding: 65px 25px;
      }

      .hero h1 {
        font-size: 48px;
      }

      .stats {
        grid-template-columns: 1fr;
      }

      .stat {
        border-right: none;
        border-bottom: 1px solid #e5e7eb;
      }

      .cards,
      .service-grid,
      .contact {
        grid-template-columns: 1fr;
      }

      .cta {
        margin: 50px 20px;
        padding: 40px 25px;
        display: block;
      }

      .cta .btn {
        margin-top: 20px;
      }
    }
  </style>
</head>

<body>

<header>
  <nav>

    <a href="#" class="logo">
      Cert<span>Pro</span>
    </a>

    <ul class="menu">
      <li><a href="#certifications">Certifications</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>

    <a href="#contact" class="nav-btn">
      Get Started
    </a>

  </nav>
</header>


<!-- HERO -->

<section class="hero">

  <div>

    <div class="tag">
      CERTIFICATION PREPARATION
    </div>

    <h1>
      Prepare smarter.<br>
      <span>Certify with confidence.</span>
    </h1>

    <p>
      Study resources, practice materials and guidance
      designed to help you prepare for professional IT
      certifications.
    </p>

    <div class="buttons">

      <a href="#certifications" class="btn primary">
        Explore Certifications
      </a>

      <a href="#services" class="btn secondary">
        Our Services
      </a>

    </div>

  </div>


  <div class="hero-card">

    <small>CERTIFICATION</small>

    <h2>PREP</h2>

    <div class="item">
      <b>Study Resources</b>
      <span>Ready</span>
    </div>

    <div class="item">
      <b>Practice</b>
      <span>Available</span>
    </div>

    <div class="item">
      <b>Guidance</b>
      <span>Support</span>
    </div>

  </div>

</section>


<!-- STATS -->

<div class="stats">

  <div class="stat">
    <strong>06+</strong>
    <span>Certification Tracks</span>
  </div>

  <div class="stat">
    <strong>24/7</strong>
    <span>Online Access</span>
  </div>

  <div class="stat">
    <strong>100%</strong>
    <span>Digital Resources</span>
  </div>

</div>


<!-- CERTIFICATIONS -->

<section class="content" id="certifications">

  <div class="section-title">

    <div class="tag">
      LEARNING PATHS
    </div>

    <h2>
      Explore Certifications
    </h2>

    <p>
      Choose a certification track and start building
      your preparation plan.
    </p>

  </div>


  <div class="cards">

    <div class="card">

      <div class="icon">AWS</div>

      <h3>
        Amazon Web Services
      </h3>

      <p>
        Cloud certification preparation resources.
      </p>

      <a href="#contact">
        Learn more →
      </a>

    </div>


    <div class="card">

      <div class="icon">CC</div>

      <h3>
        Cisco
      </h3>

      <p>
        Networking and infrastructure preparation.
      </p>

      <a href="#contact">
        Learn more →
      </a>

    </div>


    <div class="card">

      <div class="icon">+</div>

      <h3>
        CompTIA
      </h3>

      <p>
        IT, security and infrastructure study paths.
      </p>

      <a href="#contact">
        Learn more →
      </a>

    </div>


    <div class="card">

      <div class="icon">M</div>

      <h3>
        Microsoft
      </h3>

      <p>
        Microsoft technology certification tracks.
      </p>

      <a href="#contact">
        Learn more →
      </a>

    </div>


    <div class="card">

      <div class="icon">ISC</div>

      <h3>
        ISC2
      </h3>

      <p>
        Cybersecurity certification preparation.
      </p>

      <a href="#contact">
        Learn more →
      </a>

    </div>


    <div class="card">

      <div class="icon">IT</div>

      <h3>
        More Certifications
      </h3>

      <p>
        Tell us which certification you are preparing for.
      </p>

      <a href="#contact">
        Ask us →
      </a>

    </div>

  </div>

</section>


<!-- SERVICES -->

<div class="gray">

<section class="services" id="services">

  <div class="section-title">

    <div class="tag">
      WHAT WE OFFER
    </div>

    <h2>
      Prepare with CertPro
    </h2>

  </div>


  <div class="service-grid">

    <div class="service">

      <div class="service-number">
        01
      </div>

      <h3>
        Study Resources
      </h3>

      <p>
        Organized digital resources to support your
        certification preparation.
      </p>

    </div>


    <div class="service">

      <div class="service-number">
        02
      </div>

      <h3>
        Practice Materials
      </h3>

      <p>
        Practice questions and revision materials
        to test your knowledge.
      </p>

    </div>


    <div class="service">

      <div class="service-number">
        03
      </div>

      <h3>
        Preparation Guidance
      </h3>

      <p>
        Get help choosing a certification and
        planning your preparation.
      </p>

    </div>

  </div>

</section>

</div>


<!-- CTA -->

<div class="cta">

  <div>

    <div class="tag">
      READY TO START?
    </div>

    <h2>
      Build your certification journey.
    </h2>

    <p>
      Tell us what certification you're preparing for.
    </p>

  </div>

  <a href="#contact" class="btn secondary">
    Contact CertPro
  </a>

</div>


<!-- CONTACT -->

<section class="contact" id="contact">

  <div class="contact-info">

    <div class="tag">
      CONTACT
    </div>

    <h2>
      Let's talk.
    </h2>

    <p>
      Replace the sample information below with
      your real business details.
    </p>

    <br>

    <p>
      <b>Email:</b><br>
      your@email.com
    </p>

    <p>
      <b>WhatsApp:</b><br>
      +880 1XXXXXXXXX
    </p>

    <p>
      <b>Location:</b><br>
      Bangladesh
    </p>

  </div>


  <form onsubmit="sendMessage(event)">

    <input
      type="text"
      placeholder="Your name"
      required
    >

    <input
      type="email"
      placeholder="Your email"
      required
    >

    <select>
      <option>Select certification</option>
      <option>AWS</option>
      <option>Cisco</option>
      <option>CompTIA</option>
      <option>Microsoft</option>
      <option>ISC2</option>
    </select>

    <textarea
      rows="5"
      placeholder="How can we help?"
    ></textarea>

    <button class="btn primary">
      Send Enquiry
    </button>

  </form>

</section>


<!-- FOOTER -->

<footer>

  <div class="logo">
    Cert<span>Pro</span>
  </div>

  <p>
    © <span id="year"></span> CertPro.
    All rights reserved.
  </p>

  <p>
    CertPro is an independent certification
    preparation platform.
  </p>

</footer>


<script>

document.getElementById("year").textContent =
new Date().getFullYear();

function sendMessage(event) {

  event.preventDefault();

  alert(
    "Thanks! Your enquiry form is ready. Connect this form to your email or form service before launching."
  );

}

</script>

</body>
</html>
