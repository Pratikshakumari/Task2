# Task2
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- SEO Meta Tags -->
  <title>Pratiksha Kumari | Personal Portfolio</title>
  <link rel="stylesheet" href="style.css">

  <meta
    name="description"
    content="Accessible and semantic personal portfolio website of Pratiksha Kumari showcasing skills, projects, and contact details."
  />

  <meta
    name="keywords"
    content="Portfolio, HTML5, CSS3, Web Developer, Python, Java, Accessibility"
  />

  <meta name="author" content="Pratiksha Kumari" />

  <style>
    /* =========================
       GLOBAL STYLES
    ========================= */

    body {
      font-family: Arial, sans-serif;
      margin: 0;
      line-height: 1.6;
      background: #ffffff;
      color: #222222;
    }

    header,
    main,
    footer,
    section,
    article,
    nav {
      padding: 20px;
    }

    header {
      background: #f4f4f4;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
      padding: 0;
    }

    nav a {
      text-decoration: none;
      color: #0056b3;
      font-weight: bold;
    }

    nav a:hover,
    nav a:focus {
      text-decoration: underline;
    }

    section {
      margin-bottom: 40px;
    }

    article {
      border: 1px solid #ddd;
      padding: 15px;
      margin-bottom: 20px;
      border-radius: 8px;
    }

    ul {
      padding-left: 20px;
    }

    /* =========================
       ACCESSIBILITY
    ========================= */

    .skip-link {
      position: absolute;
      left: -999px;
      top: 0;
      background: #000;
      color: #fff;
      padding: 10px;
    }

    .skip-link:focus {
      left: 10px;
      z-index: 1000;
    }

    nav a:focus,
    button:focus,
    input:focus,
    textarea:focus {
      outline: 3px solid #000;
      outline-offset: 2px;
    }

    /* =========================
       FORM STYLING
    ========================= */

    form div {
      margin-bottom: 15px;
    }

    input,
    textarea,
    button {
      width: 100%;
      max-width: 500px;
      padding: 10px;
      font-size: 1rem;
    }

    button {
      cursor: pointer;
      background: #0056b3;
      color: white;
      border: none;
    }

    button:hover {
      background: #003d80;
    }

    footer {
      background: #f4f4f4;
      text-align: center;
    }
  </style>
</head>

<body>

  <!-- Skip Navigation -->
  <a href="#main-content" class="skip-link">
    Skip to main content
  </a>

  <!-- =========================
       HEADER
  ========================= -->

  <header role="banner">

    <h1>Pratiksha Kumari</h1>

    <nav aria-label="Primary Navigation">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>

  </header>

  <!-- =========================
       MAIN CONTENT
  ========================= -->

  <main id="main-content">

    <!-- HOME SECTION -->
    <section id="home" aria-labelledby="home-heading">

      <h2 id="home-heading">Home</h2>

      <p>
        Hello! I am <strong>Pratiksha Kumari</strong>,
        an aspiring frontend developer passionate about creating
        accessible, responsive, and user-friendly websites using
        modern web technologies.
      </p>

      <p>
        This portfolio showcases my skills, projects, education,
        and contact information.
      </p>

      <h3>Skills</h3>

      <ul>
        <li>HTML5</li>
        <li>CSS3</li>
        <li>Python</li>
        <li>Java</li>
        <li>Responsive Web Design</li>
      </ul>

    </section>

    <!-- PROJECTS SECTION -->
    <section id="projects" aria-labelledby="projects-heading">

      <h2 id="projects-heading">Projects</h2>

      <!-- Project 1 -->
      <article>

        <h3>Car Price Predictor</h3>

        <p>
          A machine learning project developed using Python that predicts
          car prices based on features such as company, fuel type,
          and manufacturing year.
        </p>

        <p>
          <strong>Technologies Used:</strong>
          Python, Machine Learning, Pandas
        </p>

      </article>

      <!-- Project 2 -->
      <article>

        <h3>Portfolio Website</h3>

        <p>
          A fully responsive and accessible portfolio website built using
          semantic HTML5 and CSS while following WCAG accessibility standards.
        </p>

        <p>
          <strong>Technologies Used:</strong>
          HTML5, CSS3
        </p>

      </article>

      <!-- Project 3 -->
      <article>

        <h3>Student Resume Website</h3>

        <p>
          A beginner-friendly resume website designed to showcase
          educational qualifications, skills, and achievements.
        </p>

        <p>
          <strong>Technologies Used:</strong>
          HTML, CSS
        </p>

      </article>

    </section>

    <!-- CONTACT SECTION -->
    <section id="contact" aria-labelledby="contact-heading">

      <h2 id="contact-heading">Contact</h2>

      <p>
        Feel free to contact me for collaboration, internship opportunities,
        or web development projects.
      </p>

      <p>
        I will try to respond as soon as possible.
      </p>

      <!-- Accessible Contact Form -->
      <form action="#" method="post">

        <!-- Name -->
        <div>
          <label for="name">Full Name</label>

          <input
            type="text"
            id="name"
            name="name"
            required
            aria-required="true"
            placeholder="Enter your full name"
          />
        </div>

        <!-- Email -->
        <div>
          <label for="email">Email Address</label>

          <input
            type="email"
            id="email"
            name="email"
            required
            aria-required="true"
            placeholder="Enter your email address"
          />
        </div>

        <!-- Message -->
        <div>
          <label for="message">Message</label>

          <textarea
            id="message"
            name="message"
            rows="5"
            required
            aria-required="true"
            placeholder="Write your message here"
          ></textarea>
        </div>

        <!-- Submit Button -->
        <button type="submit">
          Send Message
        </button>

      </form>

    </section>

  </main>

  <!-- =========================
       FOOTER
  ========================= -->

  <footer>

    <p>
      &copy; 2026 Pratiksha Kumari. All rights reserved.
    </p>

  </footer>

</body>
</html>

# Css Part
/* ===================================================
ADVANCED CSS3 + RESPONSIVE ARCHITECTURE
Fully Responsive Portfolio Design
=================================================== */

/* =========================
   CSS VARIABLES
========================= */

:root {
  --bg-color: #ffffff;
  --text-color: #222222;
  --primary-color: #2563eb;
  --secondary-color: #f3f4f6;
  --card-bg: #ffffff;
  --border-color: #d1d5db;
  --shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

/* Dark Mode Theme */
@media (prefers-color-scheme: dark) {
  :root {
    --bg-color: #111827;
    --text-color: #f9fafb;
    --primary-color: #60a5fa;
    --secondary-color: #1f2937;
    --card-bg: #1e293b;
    --border-color: #374151;
    --shadow: 0 4px 12px rgba(255, 255, 255, 0.08);
  }
}

/* =========================
   GLOBAL RESET
========================= */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* =========================
   BODY
========================= */

body {
  font-family: Arial, sans-serif;
  background: var(--bg-color);
  color: var(--text-color);
  line-height: 1.7;
  transition: background 0.3s ease, color 0.3s ease;
}

/* =========================
   SKIP LINK
========================= */

.skip-link {
  position: absolute;
  left: -999px;
  top: 10px;
  background: black;
  color: white;
  padding: 10px;
  z-index: 1000;
}

.skip-link:focus {
  left: 10px;
}

/* =========================
   HEADER
========================= */

header {
  background: var(--secondary-color);
  padding: 20px;
  box-shadow: var(--shadow);

  /* Flexbox */
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 15px;
}

header h1 {
  font-size: 2rem;
  color: var(--primary-color);
}

/* =========================
   NAVIGATION
========================= */

nav ul {
  list-style: none;

  /* Flexbox */
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

nav a {
  text-decoration: none;
  color: var(--text-color);
  font-weight: bold;
  transition: color 0.3s ease;
}

nav a:hover,
nav a:focus {
  color: var(--primary-color);
}

/* =========================
   MAIN LAYOUT
========================= */

main {
  padding: 20px;

  /* CSS GRID */
  display: grid;
  gap: 40px;
}

/* =========================
   SECTIONS
========================= */

section {
  background: var(--secondary-color);
  padding: 30px;
  border-radius: 16px;
  box-shadow: var(--shadow);
}

section h2 {
  margin-bottom: 20px;
  color: var(--primary-color);
  font-size: 2rem;
}

/* =========================
   HOME SECTION
========================= */

#home {
  display: grid;
  gap: 20px;
}

#home ul {
  padding-left: 20px;
}

/* =========================
   PROJECTS SECTION
========================= */

#projects {

  /* CSS GRID */
  display: grid;
  gap: 25px;
}

article {
  background: var(--card-bg);
  border: 1px solid var(--border-color);
  border-radius: 14px;
  padding: 20px;
  transition: transform 0.3s ease;
  box-shadow: var(--shadow);
}

article:hover {
  transform: translateY(-5px);
}

article h3 {
  color: var(--primary-color);
  margin-bottom: 10px;
}

/* =========================
   CONTACT SECTION
========================= */

form {

  /* Flexbox */
  display: flex;
  flex-direction: column;
  gap: 20px;
}

form div {
  display: flex;
  flex-direction: column;
}

label {
  margin-bottom: 8px;
  font-weight: bold;
}

input,
textarea {
  padding: 14px;
  border: 1px solid var(--border-color);
  border-radius: 10px;
  background: var(--card-bg);
  color: var(--text-color);
  font-size: 1rem;
}

input:focus,
textarea:focus,
button:focus,
nav a:focus {
  outline: 3px solid var(--primary-color);
  outline-offset: 2px;
}

/* =========================
   BUTTON
========================= */

button {
  padding: 14px;
  border: none;
  border-radius: 10px;
  background: var(--primary-color);
  color: white;
  font-size: 1rem;
  cursor: pointer;
  transition: background 0.3s ease;
}

button:hover {
  opacity: 0.9;
}

/* =========================
   FOOTER
========================= */

footer {
  text-align: center;
  padding: 20px;
  background: var(--secondary-color);
  margin-top: 40px;
}

/* ===================================================
   RESPONSIVE DESIGN
=================================================== */

/* =========================
   TABLET VIEW
========================= */

@media (min-width: 768px) {

  header {
    flex-direction: row;
    justify-content: space-between;
    padding: 25px 50px;
  }

  main {
    padding: 40px;
  }

  #projects {

    /* Two-column grid */
    grid-template-columns: repeat(2, 1fr);
  }

  #home {
    grid-template-columns: 1fr 1fr;
    align-items: center;
  }
}

/* =========================
   DESKTOP VIEW
========================= */

@media (min-width: 1024px) {

  body {
    font-size: 18px;
  }

  main {
    max-width: 1200px;
    margin: auto;
  }

  #projects {

    /* Three-column grid */
    grid-template-columns: repeat(3, 1fr);
  }

  section {
    padding: 40px;
  }

  header h1 {
    font-size: 2.5rem;
  }

  section h2 {
    font-size: 2.3rem;
  }
}
