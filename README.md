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
