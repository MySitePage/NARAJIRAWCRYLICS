
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Explore the creative world of Naraji Love: beauty, art, gardening, writing, and entrepreneurship.">
  <title>Naraji Love | A World of Her Own</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,500;0,600;1,400;1,500&display=swap" rel="stylesheet">

  <style>
    :root {
      --cream: #f5efe7;
      --white: #fffaf5;
      --brown: #251d1b;
      --muted: #766962;
      --wine: #702f3c;
      --rose: #d8aaa5;
      --line: #ddd0c4;
      --serif: "Playfair Display", Georgia, serif;
      --sans: "DM Sans", Arial, sans-serif;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
      scroll-padding-top: 85px;
    }

    body {
      background: var(--cream);
      color: var(--brown);
      font-family: var(--sans);
      line-height: 1.7;
    }

    img {
      display: block;
      width: 100%;
      object-fit: cover;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1200px, 90%);
      margin: auto;
    }

    .eyebrow {
      color: var(--wine);
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 3px;
      text-transform: uppercase;
    }

    h1, h2, h3 {
      font-family: var(--serif);
      font-weight: 400;
      line-height: 1.15;
    }

    h2 {
      font-size: clamp(38px, 6vw, 68px);
      letter-spacing: -2px;
    }

    p {
      color: var(--muted);
      margin: 16px 0;
    }

    /* HEADER */

    .announcement {
      padding: 8px 15px;
      background: var(--brown);
      color: white;
      text-align: center;
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(245, 239, 231, .96);
      border-bottom: 1px solid var(--line);
      backdrop-filter: blur(12px);
    }

    nav {
      min-height: 78px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 25px;
    }

    .logo {
      font-family: var(--serif);
      font-size: 27px;
      line-height: 1.1;
      white-space: nowrap;
    }

    .logo small {
      display: block;
      margin-top: 5px;
      font-family: var(--sans);
      font-size: 8px;
      letter-spacing: 3px;
      text-align: center;
      text-transform: uppercase;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 25px;
    }

    .nav-links a {
      font-size: 10px;
      letter-spacing: 1.2px;
      text-transform: uppercase;
      transition: color .2s;
    }

    .nav-links a:hover {
      color: var(--wine);
    }

    .nav-button, .button {
      display: inline-block;
      padding: 13px 20px;
      border: 1px solid var(--brown);
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      transition: .25s;
    }

    .nav-button:hover, .button:hover {
      background: var(--brown);
      color: white;
    }

    .menu-toggle {
      display: none;
      border: none;
      background: transparent;
      font-size: 27px;
      cursor: pointer;
    }

    /* HERO */

    .hero {
      padding: 28px 0 75px;
    }

    .hero-image {
      position: relative;
      min-height: 650px;
      overflow: hidden;
      display: flex;
      align-items: flex-end;
      background: #383331;
      color: white;
    }

    .hero-image::before {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(
        90deg,
        rgba(18, 16, 16, .15),
        rgba(18, 16, 16, .05) 75%
      );
      z-index: 1;
    }

    .hero-image > img {
      position: absolute;
      inset: 0;
      height: 100%;
      z-index: 0;
      object-position: center;
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 760px;
      padding: 65px;
    }

    .hero-content .eyebrow {
      color: #f2d6d0;
    }

    .hero h1 {
      margin: 20px 0;
      font-size: clamp(60px, 10vw, 115px);
      letter-spacing: -5px;
    }

    .hero h1 em {
      color: #e6bbb5;
    }

    .hero-content p {
      max-width: 480px;
      color: #f1e8e4;
      font-size: 15px;
    }

    .hero .button {
      margin-top: 18px;
      border-color: white;
      color: white;
    }

    .hero .button:hover {
      background: white;
      color: var(--brown);
    }

    .intro {
      display: grid;
      grid-template-columns: 1fr 1.5fr 1fr;
      gap: 30px;
      align-items: center;
      padding: 45px 0 65px;
      border-bottom: 1px solid var(--line);
    }

    .intro p {
      margin: 0;
      font-size: 13px;
    }

    .intro-quote {
      font-family: var(--serif);
      font-size: clamp(23px, 3vw, 36px);
      line-height: 1.4;
      text-align: center;
    }

    .intro-quote em {
      color: var(--wine);
    }

    /* GENERAL SECTIONS */

    section.content-section {
      padding: 100px 0;
    }

    .section-heading {
      display: flex;
      justify-content: space-between;
      align-items: end;
      gap: 35px;
      margin-bottom: 45px;
    }

    .section-heading h2 {
      margin-top: 15px;
    }

    .section-heading p {
      max-width: 380px;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 75px;
      align-items: center;
    }

    .portrait {
      position: relative;
      padding: 0 25px 25px 0;
    }

    .portrait::after {
      content: "";
      position: absolute;
      width: 75%;
      height: 70%;
      right: 0;
      bottom: 0;
      background: #d9b8a8;
      z-index: -1;
    }

    .portrait img {
      height: 580px;
      object-position: center 35%;
    }

    .about-copy h2 {
      margin: 15px 0 25px;
    }

    .lead {
      color: var(--brown);
      font-family: var(--serif);
      font-size: 24px;
      line-height: 1.5;
    }

    .text-link {
      display: inline-block;
      margin-top: 12px;
      padding-bottom: 6px;
      border-bottom: 1px solid var(--wine);
      color: var(--wine);
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
    }

    /* PORTFOLIO */

    .portfolio {
      background: var(--brown);
      color: white;
    }

    .portfolio .eyebrow {
      color: #e0aaa6;
    }

    .portfolio .section-heading p {
      color: #cbbeb6;
    }

    .portfolio-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 22px;
    }

    .portfolio-card {
      position: relative;
      min-height: 400px;
      overflow: hidden;
      background: #4c3d39;
      color: white;
      isolation: isolate;
    }

    .portfolio-card.tall {
      grid-row: span 2;
      min-height: 600px;
    }

    .portfolio-card > img {
      position: absolute;
      inset: 0;
      height: 100%;
      z-index: -2;
      transition: transform .6s;
    }

    .portfolio-card:hover > img {
      transform: scale(1.05);
    }

    .portfolio-card::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(
        0deg,
        rgba(20, 14, 13, .9),
        transparent 80%
      );
      z-index: -1;
    }

    .card-copy {
      position: absolute;
      right: 28px;
      bottom: 28px;
      left: 28px;
    }

    .card-number {
      color: #e7bdb6;
      font-size: 10px;
      letter-spacing: 2px;
    }

    .portfolio-card h3 {
      margin: 12px 0;
      font-size: clamp(27px, 3vw, 40px);
    }

    .portfolio-card p {
      max-width: 400px;
      color: #f0e7e1;
      font-size: 13px;
    }

    /* NAIL FEATURE */

    .nail-section {
      background: var(--white);
    }

    .nail-photo {
      padding: 18px;
      background: #e8d8cb;
    }

    .nail-photo img {
      height: 480px;
    }

    .shea-gallery {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin: 30px 0;
    }

    .shea-gallery img {
      width: 100%;
      height: auto;
      border: 8px solid #e8d8cb;
    }

    /* QUOTE */

    .quote-section {
      padding: 90px 20px;
      background: #e9dcd0;
      text-align: center;
    }

    .quote-section h2 {
      max-width: 850px;
      margin: 25px auto;
      font-size: clamp(35px, 5.5vw, 65px);
    }

    .quote-section h2 em {
      color: var(--wine);
    }

    .signature {
      color: var(--wine);
      font-family: var(--serif);
      font-size: 20px;
      font-style: italic;
    }

    /* BOOKS */

    .books-grid {
      display: grid;
      grid-template-columns: .8fr 1.2fr;
      gap: 65px;
      align-items: center;
    }

    .book-display {
      min-height: 480px;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 35px;
      background: #ddc9b7;
    }

    .book-cover {
      width: 275px;
      min-height: 395px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding: 35px 25px;
      background: #354537;
      color: #f6ead9;
      text-align: center;
      box-shadow: 15px 17px 0 rgba(40, 28, 23, .13);
      transform: rotate(-3deg);
    }

    .book-cover .small {
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    .book-cover .leaf {
      font-size: 42px;
      color: #c6c9a5;
    }

    .book-cover .title {
      font-family: var(--serif);
      font-size: 43px;
      line-height: 1.05;
    }

    .book-cover .title em {
      color: #d9bd8e;
    }

    /* Actual book cover image display */
    .book-cover-img {
      width: 275px;
      box-shadow: 15px 17px 0 rgba(40, 28, 23, .13);
      transform: rotate(-3deg);
      border: 0;
    }

    .book-cover-img img {
      width: 100%;
      height: auto;
    }

    .book-item {
      padding: 22px 0;
      border-bottom: 1px solid var(--line);
    }

    .book-item:last-child {
      border-bottom: 0;
    }

    .book-item .status {
      color: var(--wine);
      font-size: 9px;
      font-weight: 700;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    .book-item h3 {
      margin: 9px 0;
      font-size: 27px;
    }

    .book-item p {
      font-size: 13px;
    }

    /* OTHER CREATIVE WORK */

    .nature-section {
      background: #e9e0d6;
    }

    .nature-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1px;
      margin-top: 35px;
      border: 1px solid #d4c6b9;
      background: #d4c6b9;
    }

    .nature-card {
      padding: 32px;
      background: #e9e0d6;
    }

    .nature-card .number {
      color: var(--wine);
      font-size: 10px;
      letter-spacing: 2px;
    }

    .nature-card h3 {
      margin: 20px 0 10px;
      font-size: 27px;
    }

    .nature-card p {
      font-size: 13px;
    }

    /* CONTACT */

    .contact {
      padding: 90px 0;
      background: var(--wine);
      color: white;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1.2fr .8fr;
      gap: 60px;
      align-items: end;
    }

    .contact .eyebrow {
      color: #f0c9c2;
    }

    .contact h2 {
      margin: 15px 0 25px;
      font-size: clamp(55px, 8vw, 90px);
    }

    .contact p {
      max-width: 450px;
      color: #eadbd7;
    }

    .contact .button {
      margin-top: 15px;
      border-color: white;
      color: white;
    }

    .contact .button:hover {
      background: white;
      color: var(--wine);
    }

    .contact-links {
      display: flex;
      flex-direction: column;
      gap: 17px;
    }

    .contact-links a {
      padding-bottom: 8px;
      border-bottom: 1px solid #b77f85;
      color: #f8e9e4;
      font-size: 12px;
    }

    .contact-links .ig-link {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .contact-links .ig-icon {
      width: 16px;
      height: 16px;
      flex-shrink: 0;
      color: #f8e9e4;
      transition: color .2s, transform .2s;
    }

    .contact-links .ig-link:hover .ig-icon {
      color: white;
      transform: scale(1.1);
    }

    footer {
      padding: 25px 0;
      background: #1c1716;
      color: #d8c9c0;
      font-size: 10px;
      letter-spacing: 1px;
    }

    .footer-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
    }

    .footer-logo {
      font-family: var(--serif);
      font-size: 21px;
      letter-spacing: 0;
    }

    /* ===== FULL-SCREEN GALLERY OVERLAYS ===== */

    .gallery-overlay {
      display: none;
      position: fixed;
      inset: 0;
      z-index: 999;
      background: var(--cream);
      overflow-y: auto;
    }

    .gallery-overlay.active {
      display: block;
    }

    .gallery-overlay-header {
      position: sticky;
      top: 0;
      z-index: 10;
      background: rgba(245, 239, 231, .97);
      border-bottom: 1px solid var(--line);
      backdrop-filter: blur(12px);
    }

    .gallery-overlay-nav {
      min-height: 78px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 25px;
    }

    .gallery-overlay-nav .logo {
      font-family: var(--serif);
      font-size: 27px;
      line-height: 1.1;
      white-space: nowrap;
    }

    .gallery-overlay-nav .logo small {
      display: block;
      margin-top: 5px;
      font-family: var(--sans);
      font-size: 8px;
      letter-spacing: 3px;
      text-align: center;
      text-transform: uppercase;
    }

    .close-gallery {
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      padding: 13px 20px;
      border: 1px solid var(--brown);
      background: transparent;
      color: var(--brown);
      font-family: var(--sans);
      cursor: pointer;
      transition: .25s;
    }

    .close-gallery:hover {
      background: var(--brown);
      color: white;
    }

    .gallery-overlay-intro {
      padding: 70px 0 40px;
      text-align: center;
    }

    .gallery-overlay-intro h1 {
      font-size: clamp(44px, 8vw, 88px);
      letter-spacing: -3px;
      margin: 18px 0;
    }

    .gallery-overlay-intro h1 em {
      color: var(--wine);
    }

    .gallery-overlay-intro p {
      max-width: 560px;
      margin: 0 auto;
    }

    .gallery-overlay-body {
      padding: 20px 0 80px;
    }

    .overlay-grid-masonry {
      columns: 3;
      column-gap: 20px;
    }

    .overlay-grid-masonry .gallery-item {
      break-inside: avoid;
      margin-bottom: 20px;
    }

    .overlay-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .gallery-item {
      overflow: hidden;
      background: #e8d8cb;
    }

    .gallery-item img {
      transition: transform .6s;
    }

    .gallery-item:hover img {
      transform: scale(1.05);
    }

    .gallery-overlay-cta {
      padding: 70px 0;
      background: var(--wine);
      color: white;
      text-align: center;
    }

    .gallery-overlay-cta .eyebrow {
      color: #f0c9c2;
    }

    .gallery-overlay-cta h2 {
      margin: 15px 0 25px;
      font-size: clamp(34px, 5vw, 60px);
    }

    .gallery-overlay-cta h2 em {
      color: #e6bbb5;
    }

    .gallery-overlay-cta p {
      max-width: 480px;
      margin: 0 auto 25px;
      color: #eadbd7;
    }

    .gallery-overlay-cta .button {
      border-color: white;
      color: white;
    }

    .gallery-overlay-cta .button:hover {
      background: white;
      color: var(--wine);
    }

    @media (max-width: 900px) {
      .nav-links {
        gap: 12px;
      }

      .nav-links a {
        font-size: 9px;
      }

      .nav-button {
        display: none;
      }

      .hero-image {
        min-height: 560px;
      }

      .hero-content {
        padding: 40px;
      }

      .intro {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .about-grid,
      .books-grid,
      .contact-grid {
        grid-template-columns: 1fr;
        gap: 40px;
      }

      .portrait {
        max-width: 600px;
      }

      .nature-grid {
        grid-template-columns: 1fr;
      }

      .overlay-grid-masonry {
        columns: 2;
      }

      .overlay-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 600px) {
      .container {
        width: 90%;
      }

      nav {
        min-height: 70px;
      }

      .logo {
        font-size: 24px;
      }

      .menu-toggle {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 70px;
        left: 0;
        right: 0;
        padding: 25px;
        background: var(--cream);
        border-bottom: 1px solid var(--line);
        flex-direction: column;
        align-items: flex-start;
      }

      .nav-links.open {
        display: flex;
      }

      .nav-links a {
        font-size: 11px;
      }

      .hero {
        padding-top: 15px;
      }

      .hero-image {
        min-height: 570px;
      }

      .hero-content {
        padding: 25px;
      }

      .hero h1 {
        font-size: 60px;
        letter-spacing: -3px;
      }

      section.content-section {
        padding: 70px 0;
      }

      .section-heading {
        flex-direction: column;
        align-items: flex-start;
        gap: 10px;
      }

      .portfolio-grid {
        grid-template-columns: 1fr;
      }

      .portfolio-card,
      .portfolio-card.tall {
        grid-row: auto;
        min-height: 430px;
      }

      .portrait img {
        height: 450px;
      }

      .nail-photo img {
        height: 350px;
      }

      .book-display {
        min-height: 430px;
      }

      .footer-row {
        flex-direction: column;
        text-align: center;
      }

      .shea-gallery {
        grid-template-columns: 1fr;
      }

      .overlay-grid-masonry {
        columns: 1;
      }

      .overlay-grid {
        grid-template-columns: 1fr;
      }

      .gallery-overlay-nav {
        min-height: 70px;
      }
    }
  </style>
</head>

<body>

  <div class="announcement">
    Beauty · Art · Nature · Words · Purpose
  </div>

  <header>
    <nav class="container">
      <a href="#home" class="logo">
        Naraji Love
        <small>A creative portfolio</small>
      </a>

      <button class="menu-toggle" aria-label="Open navigation"
        aria-expanded="false">☰</button>

      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#work">Portfolio</a>
        <a href="#nails">Beauty</a>
        <a href="#books">Books</a>
        <a href="#garden">Nature</a>
        <a href="#contact">Contact</a>
      </div>

      <a class="nav-button" href="#contact">Let's Connect ↗</a>
    </nav>
  </header>

  <main>

    <!-- HERO IMAGE -->
    <section class="hero container" id="home">
      <div class="hero-image">
        <img
          src="https://i.postimg.cc/9FyrbM9L/Screenshot-2026-03-24-094423.png"
          alt="Naraji Love portfolio hero image"
          fetchpriority="high">

        <div class="hero-content">
          <div class="eyebrow">An independent creative spirit</div>

          <h1>A World<br>of <em>Her Own.</em></h1>

          <p>
            Beauty, art, nature, and ideas — a growing collection of
            passions brought together through creativity and purpose.
          </p>

          <a class="button" href="#work">Explore Her World ↗</a>
        </div>
      </div>

      <div class="intro">
        <p class="eyebrow">One woman. Many expressions.</p>

        <div class="intro-quote">
          Creativity takes many forms.<br>
          <em>Every one tells a story.</em>
        </div>

        <p>
          Welcome to the creative world of Naraji Love, where curiosity
          meets craftsmanship and ideas have room to grow.
        </p>
      </div>
    </section>

    <!-- ABOUT -->
    <section class="content-section container" id="about">
      <div class="about-grid">
        <div class="portrait">
          <img
            src="https://i.postimg.cc/26p4yJNy/Screenshot-2026-03-25-103448.png"
            alt="Naraji Love model portrait">
        </div>

        <div class="about-copy">
          <div class="eyebrow">01 / Meet Naraji</div>

          <h2>More than one<br><em>kind of creative.</em></h2>

          <p class="lead">
            A curious mind, an artistic spirit, and a vision that
            continues to grow.
          </p>

          <p>
            Naraji Love is a multidisciplinary creative exploring
            beauty, visual art, gardening, writing, modeling, and
            entrepreneurship.
          </p>

          <p>
            From the precision of a nail design to a garden taking
            shape or a manuscript growing from an idea, she enjoys
            learning, experimenting, and discovering new ways to create.
          </p>

          <p>
            Her work brings together personal expression, curiosity,
            and a desire to build something meaningful.
          </p>

          <a class="text-link" href="#work">Discover Her Work →</a>
        </div>
      </div>
    </section>

    <!-- PORTFOLIO -->
    <section class="content-section portfolio" id="work">
      <div class="container">
        <div class="section-heading">
          <div>
            <div class="eyebrow">02 / Selected disciplines</div>
            <h2>Different worlds.<br><em>One point of view.</em></h2>
          </div>

          <p>
            Explore the different creative areas Naraji is developing,
            each with its own materials, inspiration, and possibilities.
          </p>
        </div>

        <div class="portfolio-grid">

          <!-- NAIL PHOTO — opens full-screen nails gallery -->
          <a class="portfolio-card tall" href="#nails-gallery" data-gallery="nails">
            <img
              src="https://i.postimg.cc/RZ7m2JC1/Screenshot-2026-03-24-094622.png"
              alt="NarajiRawCrylics nail art portfolio"
              loading="lazy">

            <div class="card-copy">
              <div class="card-number">01 / BEAUTY & NAIL ART</div>
              <h3>NarajiRawCrylics</h3>
              <p>
                Acrylics, Gel-X, press-on designs, and beauty expressed
                through color, shape, and detail.
              </p>
              <span>Explore Beauty ↗</span>
            </div>
          </a>

          <!-- EXTRA PHOTO — opens full-screen nature gallery -->
          <a class="portfolio-card" href="#nature-gallery" data-gallery="nature">
            <img
              src="https://i.postimg.cc/QtbHDn83/Screenshot-2026-03-24-094333.png"
              alt="Creative work selected for Naraji Love's portfolio"
              loading="lazy">

            <div class="card-copy">
              <div class="card-number">02 / NATURE & GROWING</div>
              <h3>Rooted in Curiosity</h3>
              <p>
                Gardening, plants, propagation, and learning through
                the natural world.
              </p>
              <span>Explore Nature ↗</span>
            </div>
          </a>

          <!-- BOOKS — opens full-screen books gallery -->
          <a class="portfolio-card" href="#books-gallery" data-gallery="books">
            <img
              src="https://i.postimg.cc/J0sBRVpM/download.png"
              alt="The Living World book cover"
              loading="lazy">

            <div class="card-copy">
              <div class="card-number">03 / WRITING & PUBLISHING</div>
              <h3>Ideas Into Pages</h3>
              <p>
                Educational manuscripts and writing shaped by
                observation, research, and imagination.
              </p>
              <span>Explore Books ↗</span>
            </div>
          </a>

          <a class="portfolio-card" href="#vision">
            <div class="card-copy">
              <div class="card-number">04 / ART & EXPRESSION</div>
              <h3>Feeling, Form & Meaning</h3>
              <p>
                Visual art, poetry, styling, and creative
                spaces that tell a story.
              </p>
              <span>Discover Her Vision ↗</span>
            </div>
          </a>

        </div>
      </div>
    </section>

    <!-- NAILS -->
    <section class="content-section nail-section" id="nails">
      <div class="container">
        <div class="section-heading">
          <div>
            <div class="eyebrow">03 / Beauty studio</div>
            <h2>Detail is its<br><em>own language.</em></h2>
          </div>

          <p>
            Beauty becomes a space for individuality, where finish,
            proportion, color, and tiny details all matter.
          </p>
        </div>

        <div class="about-grid">
          <div class="about-copy">
            <p class="lead">
              A creative practice built around technique and individuality.
            </p>

            <p>
              Through NarajiRawCrylics, Naraji explores acrylic nails,
              Gel-X, press-on designs, and toe services.
            </p>

            <p>
              She is developing a stronger focus on press-on nails,
              creating designs that can reach beyond individual
              appointments.
            </p>

            <p>
              Her goal is to continue refining her craft and creating
              thoughtful designs from the first idea to the final finish.
            </p>

            <a class="text-link" href="#contact">Beauty Inquiries →</a>
          </div>

          <div class="nail-photo">
            <img
              src="https://i.postimg.cc/RZ7m2JC1/Screenshot-2026-03-24-094622.png"
              alt="Nail design by NarajiRawCrylics"
              loading="lazy">
          </div>
        </div>
      </div>
    </section>

    <!-- SHEA BUTTER / NATURAL PRODUCTS FEATURE -->
    <section class="content-section nail-section" id="shea">
      <div class="container">
        <div class="section-heading">
          <div>
            <div class="eyebrow">Naraji Raw Organics</div>
            <h2>From plant<br><em>to product.</em></h2>
          </div>

          <p>
            Her shea butter business is part of Naraji Raw Organics —
            thoughtful, plant-based body care made with care.
          </p>
        </div>

        <div class="about-grid">
          <div class="about-copy">
            <p class="lead">
              Nourishing shea butter, made with intention.
            </p>

            <p>
              Through Naraji Raw Organics, Naraji is building a line of
              natural body butters, hair oils, and plant-based products.
            </p>

            <p>
              Her shea butter creations focus on rich, skin-loving
              ingredients, careful formulation, and thoughtful
              presentation from jar to label.
            </p>

            <a class="text-link" href="#contact">Product Inquiries →</a>
          </div>

          <div class="shea-gallery">
            <img
              src="https://i.postimg.cc/MKqK9Hrb/Screenshot-20260405-201239-Docs-2.jpg"
              alt="Naraji Raw Organics shea butter product photo"
              loading="lazy">
            <img
              src="https://i.postimg.cc/yYsYLxrh/Screenshot-20260405-201153-Docs-2.jpg"
              alt="Naraji Raw Organics shea butter product photo"
              loading="lazy">
          </div>
        </div>
      </div>
    </section>

    <!-- QUOTE -->
    <section class="quote-section">
      <div class="eyebrow">The philosophy</div>

      <h2>
        Make room for the idea.<br>
        Give it the <em>care</em> to grow.
      </h2>

      <div class="signature">— Naraji Love</div>
    </section>

    <!-- BOOKS -->
    <section class="content-section container" id="books">
      <div class="books-grid">

        <div class="book-display">
          <div class="book-cover-img">
            <img
              src="https://i.postimg.cc/J0sBRVpM/download.png"
              alt="The Living World book cover by Naraji Love"
              loading="lazy">
          </div>
        </div>

        <div>
          <div class="eyebrow">04 / Books & publishing</div>

          <h2>Research with<br>a little <em>wonder.</em></h2>

          <p>
            Naraji's writing brings together curiosity, observation,
            and accessible explanations. Her developing manuscripts
            aim to make complex subjects inviting and informative.
          </p>

          <div class="book-item">
            <div class="status">In development · Educational</div>
            <h3>The Living World</h3>
            <p>
              An introduction to plant science for younger readers,
              exploring seeds, germination, roots, stems, leaves,
              photosynthesis, flowers, and plant reproduction.
            </p>
          </div>

          <div class="book-item">
            <div class="status">In development · Plant science</div>
            <h3>Where the Flower Keeps Its Fire</h3>
            <p>
              A developing manuscript exploring the life and chemistry
              of cannabis through plant science and research.
            </p>
          </div>

          <p>
            Publishing vision: Naraji Love Publishing.
          </p>
        </div>

      </div>
    </section>

    <!-- GARDENING AND PRODUCTS -->
    <section class="content-section nature-section" id="garden">
      <div class="container">
        <div class="section-heading">
          <div>
            <div class="eyebrow">05 / Nature, products & spaces</div>
            <h2>Ideas that take<br><em>root.</em></h2>
          </div>

          <p>
            From growing plants to developing natural products,
            creativity can live far beyond a canvas or a page.
          </p>
        </div>

        <div class="nature-grid">

          <article class="nature-card">
            <div class="number">A / GARDENING</div>
            <h3>Grow With Intention</h3>
            <p>
              Raised beds, fruit and herbs, trellises, propagation
              systems, plant science, and ideas for garden builds.
            </p>
          </article>

          <article class="nature-card">
            <div class="number">B / NATURAL PRODUCTS</div>
            <h3>From Plant to Product</h3>
            <p>
              Through Naraji Raw Organics, she is exploring body
              butters, hair oils, plant-based ingredients, and
              thoughtful product presentation.
            </p>
          </article>

          <article class="nature-card">
            <div class="number">C / ART & SPACES</div>
            <h3>Make a Feeling Visible</h3>
            <p>
              Poetry, interior styling, and garden design
              offer ways to experiment with atmosphere, composition,
              and personal expression.
            </p>
          </article>

        </div>
      </div>
    </section>

    <!-- VISION -->
    <section class="content-section container" id="vision">
      <div class="about-grid">
        <div class="about-copy">
          <div class="eyebrow">06 / Her point of view</div>

          <h2>Purpose in the<br><em>process.</em></h2>

          <p class="lead">
            Curiosity is the thread that connects the work.
          </p>

          <p>
            Naraji's visual art and poetry explore emotion, identity,
            nature, and the meanings that can sit beneath the surface.
          </p>

          <p>
            Her wider vision brings her creative interests and ventures
            together under Naraji Love Enterprises LLC, including
            Naraji Love Publishing.
          </p>

          <p>
            Faith, personal growth, and a desire to live purposefully
            also inform the person she is becoming and the work she
            hopes to share.
          </p>
        </div>

        <div class="portrait">
          <img
            src="https://i.postimg.cc/d1VX0L24/Screenshot-2026-03-24-094353.png"
            alt="Naraji Love portrait"
            loading="lazy">
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section class="contact" id="contact">
      <div class="container contact-grid">
        <div>
          <div class="eyebrow">07 / Contact & collaborations</div>

          <h2>Have an idea<br>in mind?</h2>

          <p>
            For creative collaborations, beauty inquiries, publishing
            questions, or conversations about her work, reach out
            and start a conversation.
          </p>

          <a class="button" href="mailto:narajilove@gmail.com">
            Start a Conversation ↗
          </a>
        </div>

        <div class="contact-links">
          <div class="eyebrow">Explore & connect</div>

          <a href="mailto:narajilove@gmail.com">narajilove@gmail.com</a>
          <a href="tel:+17862514782">(786) 251-4782</a>

          <a href="https://instagram.com/NarajiRawcrylics" target="_blank" rel="noopener" class="ig-link">
            <svg class="ig-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
              <rect x="2.5" y="2.5" width="19" height="19" rx="5"></rect>
              <circle cx="12" cy="12" r="4.2"></circle>
              <circle cx="17.4" cy="6.6" r="1.1" fill="currentColor" stroke="none"></circle>
            </svg>
            @NarajiRawcrylics
          </a>

          <a href="https://instagram.com/NarajiRaworganic" target="_blank" rel="noopener" class="ig-link">
            <svg class="ig-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
              <rect x="2.5" y="2.5" width="19" height="19" rx="5"></rect>
              <circle cx="12" cy="12" r="4.2"></circle>
              <circle cx="17.4" cy="6.6" r="1.1" fill="currentColor" stroke="none"></circle>
            </svg>
            @NarajiRaworganic
          </a>

          <a href="#nails">NarajiRawCrylics — Beauty & Nails ↗</a>
          <a href="#books">Naraji Love Publishing — Books ↗</a>
          <a href="#shea">Naraji Raw Organics — Natural Products ↗</a>
          <a href="#vision">Art, Poetry & Creative Projects ↗</a>
        </div>
      </div>
    </section>

  </main>

  <!-- FOOTER -->
  <footer>
    <div class="container footer-row">
      <div class="footer-logo">Naraji Love</div>
      <div>Beauty · Art · Nature · Words</div>
      <div>
        © <span id="year"></span> Naraji Love Enterprises LLC
      </div>
    </div>
  </footer>

  <!-- ============ NAILS GALLERY OVERLAY ============ -->
  <div class="gallery-overlay" id="nails-gallery">
    <div class="gallery-overlay-header">
      <div class="container gallery-overlay-nav">
        <a href="#" class="logo">
          Naraji Love
          <small>NarajiRawCrylics</small>
        </a>
        <button class="close-gallery" data-close>← Back to Portfolio</button>
      </div>
    </div>

    <div class="gallery-overlay-intro container">
      <div class="eyebrow">01 / Beauty & Nail Art</div>
      <h1>Nail <em>Art</em> Gallery</h1>
      <p>
        Acrylics, Gel-X, press-on designs, and toe services — a collection
        of work where color, shape, and tiny details tell the story.
      </p>
    </div>

    <div class="gallery-overlay-body container">
      <div class="overlay-grid-masonry">

        <div class="gallery-item">
          <img src="https://i.postimg.cc/RZ7m2JC1/Screenshot-2026-03-24-094622.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/25hjx9gf/Screenshot-2026-03-24-094410.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/hjnDZbqq/Screenshot-2026-03-24-094458.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/HxmYv4CG/Screenshot-2026-03-24-094513.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/fLszqjhn/Screenshot-2026-03-24-094527.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/7L0PNtjD/Screenshot-2026-03-24-094558.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/43V412jg/Screenshot-2026-03-24-094645.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/yNc6Tp2s/Screenshot-2026-03-24-094709.png"
            alt="Nail art by NarajiRawCrylics" loading="lazy">
        </div>

      </div>
    </div>

    <div class="gallery-overlay-cta">
      <div class="container">
        <div class="eyebrow">Beauty Inquiries</div>
        <h2>Want a set of <em>your own?</em></h2>
        <p>
          Reach out for press-on designs, Gel-X, acrylics, and custom
          sets through NarajiRawCrylics.
        </p>
        <a class="button" href="mailto:narajilove@gmail.com">Start a Conversation ↗</a>
      </div>
    </div>
  </div>

  <!-- ============ NATURE GALLERY OVERLAY ============ -->
  <div class="gallery-overlay" id="nature-gallery">
    <div class="gallery-overlay-header">
      <div class="container gallery-overlay-nav">
        <a href="#" class="logo">
          Naraji Love
          <small>Rooted in Curiosity</small>
        </a>
        <button class="close-gallery" data-close>← Back to Portfolio</button>
      </div>
    </div>

    <div class="gallery-overlay-intro container">
      <div class="eyebrow">02 / Nature & Growing</div>
      <h1>Rooted in <em>Curiosity</em></h1>
      <p>
        Gardening, plants, propagation, and learning through the natural
        world — a look at the growing side of Naraji's creative life.
      </p>
    </div>

    <div class="gallery-overlay-body container">
      <div class="overlay-grid">

        <div class="gallery-item">
          <img src="https://i.postimg.cc/QtbHDn83/Screenshot-2026-03-24-094333.png"
            alt="Nature and gardening by Naraji Love" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/mDgqrtYV/Screenshot-2026-03-25-093836.png"
            alt="Nature and gardening by Naraji Love" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/DwrhR4fr/Screenshot-2026-03-24-094307.png"
            alt="Nature and gardening by Naraji Love" loading="lazy">
        </div>

      </div>
    </div>

    <div class="gallery-overlay-cta">
      <div class="container">
        <div class="eyebrow">Grow With Intention</div>
        <h2>Ideas that take <em>root.</em></h2>
        <p>
          From raised beds and herbs to propagation and plant science,
          follow along as the garden keeps growing.
        </p>
        <a class="button" href="mailto:narajilove@gmail.com">Get in Touch ↗</a>
      </div>
    </div>
  </div>

  <!-- ============ BOOKS GALLERY OVERLAY ============ -->
  <div class="gallery-overlay" id="books-gallery">
    <div class="gallery-overlay-header">
      <div class="container gallery-overlay-nav">
        <a href="#" class="logo">
          Naraji Love
          <small>Ideas Into Pages</small>
        </a>
        <button class="close-gallery" data-close>← Back to Portfolio</button>
      </div>
    </div>

    <div class="gallery-overlay-intro container">
      <div class="eyebrow">03 / Writing & Publishing</div>
      <h1>Ideas Into <em>Pages</em></h1>
      <p>
        Educational manuscripts and writing shaped by observation,
        research, and imagination — a look at the books in development
        through Naraji Love Publishing.
      </p>
    </div>

    <div class="gallery-overlay-body container">
      <div class="overlay-grid">

        <div class="gallery-item">
          <img src="https://i.postimg.cc/J0sBRVpM/download.png"
            alt="The Living World book cover by Naraji Love" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/J0sBRVpM/download.png"
            alt="The Living World book cover by Naraji Love" loading="lazy">
        </div>
        <div class="gallery-item">
          <img src="https://i.postimg.cc/MHnjz29w/download-(1).png"
            alt="Where the Flower Keeps Its Fire book cover by Naraji Love" loading="lazy">
        </div>

      </div>
    </div>

    <div class="gallery-overlay-cta">
      <div class="container">
        <div class="eyebrow">Naraji Love Publishing</div>
        <h2>Research with a little <em>wonder.</em></h2>
        <p>
          For publishing questions, manuscript inquiries, or
          collaborations, reach out and start a conversation.
        </p>
        <a class="button" href="mailto:narajilove@gmail.com">Get in Touch ↗</a>
      </div>
    </div>
  </div>

  <script>
    /* Mobile nav */
    const menuButton = document.querySelector(".menu-toggle");
    const navLinks = document.querySelector(".nav-links");

    menuButton.addEventListener("click", function () {
      const isOpen = navLinks.classList.toggle("open");
      menuButton.setAttribute("aria-expanded", String(isOpen));
      menuButton.textContent = isOpen ? "×" : "☰";
    });

    navLinks.querySelectorAll("a").forEach(function (link) {
      link.addEventListener("click", function () {
        navLinks.classList.remove("open");
        menuButton.setAttribute("aria-expanded", "false");
        menuButton.textContent = "☰";
      });
    });

    /* Year */
    document.getElementById("year").textContent =
      new Date().getFullYear();

    /* ===== Gallery overlay logic ===== */
    function openGallery(id) {
      const overlay = document.getElementById(id);
      if (!overlay) return;
      overlay.classList.add("active");
      overlay.scrollTop = 0;
      document.body.style.overflow = "hidden";
    }

    function closeGalleries() {
      document.querySelectorAll(".gallery-overlay.active").forEach(function (o) {
        o.classList.remove("active");
      });
      document.body.style.overflow = "";
    }

    /* Open on portfolio card click */
    document.querySelectorAll("[data-gallery]").forEach(function (card) {
      card.addEventListener("click", function (e) {
        e.preventDefault();
        const target = card.getAttribute("data-gallery");
        openGallery(target + "-gallery");
      });
    });

    /* Close buttons */
    document.querySelectorAll("[data-close]").forEach(function (btn) {
      btn.addEventListener("click", function (e) {
        e.preventDefault();
        closeGalleries();
      });
    });

    /* Allow hash links like #nails-gallery to open directly */
    function handleHash() {
      const hash = window.location.hash.replace("#", "");
      if (hash === "nails-gallery" || hash === "nature-gallery" || hash === "books-gallery") {
        closeGalleries();
        openGallery(hash);
      }
    }

    window.addEventListener("hashchange", handleHash);
    handleHash();

    /* Escape key closes gallery */
    document.addEventListener("keydown", function (e) {
      if (e.key === "Escape") closeGalleries();
    });
  </script>

</body>
</html>
