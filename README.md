# Klaus.racing
<!DOCTYPE html><html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Klaus Racing</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #1c1c1c;
      color: #fff;
    }
    header, footer {
      background-color: #000;
      padding: 1rem;
      text-align: center;
    }
    nav a {
      margin: 0 1rem;
      color: red;
      text-decoration: none;
    }
    section {
      padding: 2rem;
    }
    .language-switch {
      position: absolute;
      top: 1rem;
      right: 1rem;
    }
    .offer {
      background: #2a2a2a;
      margin: 1rem 0;
      padding: 1rem;
      border-left: 5px solid green;
    }
    .image-placeholder {
      width: 100%;
      height: 200px;
      background-color: #444;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #ccc;
    }
  </style>
</head>
<body>
  <div class="language-switch">
    <button onclick="setLanguage('de')">DE</button>
    <button onclick="setLanguage('en')">EN</button>
  </div>  <header>
    <h1 id="title">Klaus Racing</h1>
    <nav>
      <a href="#about" id="nav-about">Über uns</a>
      <a href="#offers" id="nav-offers">Angebote</a>
      <a href="#calendar" id="nav-calendar">Kalender</a>
      <a href="#contact" id="nav-contact">Kontakt</a>
    </nav>
  </header>  <section id="about">
    <h2 id="about-title">Unser Team</h2>
    <div class="image-placeholder">[Hier kommt dein Teamfoto]</div>
    <p id="about-text">Wir sind ein engagiertes Team mit Leidenschaft für Rennsport und Sim Racing.</p>
  </section>  <section id="offers">
    <h2 id="offers-title">Coaching Angebote</h2>
    <div class="offer">
      <h3>30 Minuten</h3>
      <p id="offer-30">Renn- oder Sim-Racing-Coaching – kurz und effektiv.</p>
    </div>
    <div class="offer">
      <h3>1 Stunde</h3>
      <p id="offer-60">Ausführliches Coaching für nachhaltige Verbesserung.</p>
    </div>
    <div class="offer">
      <h3>2 Stunden</h3>
      <p id="offer-120">Intensives Training mit Analyse und Praxis.</p>
    </div>
  </section>  <section id="calendar">
    <h2 id="calendar-title">Kalender</h2>
    <div class="image-placeholder">[Hier kannst du später deinen Kalender einfügen]</div>
  </section>  <section id="contact">
    <h2 id="contact-title">Kontakt</h2>
    <p id="contact-text">Du kannst uns erreichen per:</p>
    <p>Email: <a href="mailto:info@klaus-racing.de">info@klaus-racing.de</a></p>
    <p>Telefon: +49 123 456789</p>
  </section>  <footer>
    &copy; 2025 Klaus Racing
  </footer>  <script>
    const translations = {
      en: {
        title: "Klaus Racing",
        "nav-about": "About Us",
        "nav-offers": "Offers",
        "nav-calendar": "Schedule",
        "nav-contact": "Contact",
        "about-title": "Our Team",
        "about-text": "We are a dedicated team with a passion for racing and sim racing.",
        "offers-title": "Coaching Offers",
        "offer-30": "Race or sim racing coaching – short and effective.",
        "offer-60": "Detailed coaching for lasting improvement.",
        "offer-120": "Intensive training with analysis and practice.",
        "calendar-title": "Schedule",
        "contact-title": "Contact",
        "contact-text": "You can reach us via:"
      },
      de: {
        title: "Klaus Racing",
        "nav-about": "Über uns",
        "nav-offers": "Angebote",
        "nav-calendar": "Kalender",
        "nav-contact": "Kontakt",
        "about-title": "Unser Team",
        "about-text": "Wir sind ein engagiertes Team mit Leidenschaft für Rennsport und Sim Racing.",
        "offers-title": "Coaching Angebote",
        "offer-30": "Renn- oder Sim-Racing-Coaching – kurz und effektiv.",
        "offer-60": "Ausführliches Coaching für nachhaltige Verbesserung.",
        "offer-120": "Intensives Training mit Analyse und Praxis.",
        "calendar-title": "Kalender",
        "contact-title": "Kontakt",
        "contact-text": "Du kannst uns erreichen per:"
      }
    };

    function setLanguage(lang) {
      for (const id in translations[lang]) {
        document.getElementById(id).textContent = translations[lang][id];
      }
    }
  </script></body>
</html>
