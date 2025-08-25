<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Your Name — Portfolio</title>
  <meta name="description" content="Personal website and portfolio for Your Name: projects, resume, and links." />
  <meta property="og:title" content="Your Name — Portfolio" />
  <meta property="og:description" content="Projects, resume, and links." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="photo.jpg" />
  <meta name="theme-color" content="#0ea5e9" />
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='50' fill='%230ea5e9'/%3E%3Ctext x='50' y='58' text-anchor='middle' font-size='54' font-family='Arial' fill='white'%3EY%3C/text%3E%3C/svg%3E" />
  <style>
    :root {
      --bg: #0b0c10;/* used in dark mode */
      --bg-light: #ffffff;
      --text: #0f172a;
      --muted: #475569;
      --brand: #0ea5e9; /* sky-500 */
      --brand-dark: #0284c7; /* sky-600 */
      --card: #f8fafc;
      --ring: rgba(14, 165, 233, 0.25);
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg-light: #0b0c10;
        --text: #e2e8f0;
        --muted: #94a3b8;
        --card: #111827;
      }
    }
    * { box-sizing: border-box; }
    body { margin: 0; font-family: system-ui, -apple-system, Segoe UI, Roboto, Inter, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji"; color: var(--text); background: var(--bg-light); line-height: 1.6; }
    a { color: var(--brand); text-decoration: none; }
    a:hover { text-decoration: underline; }
    .container { max-width: 960px; margin: 0 auto; padding: 24px; }
    header { position: sticky; top: 0; backdrop-filter: saturate(1.2) blur(6px); background: color-mix(in oklab, var(--bg-light), transparent 35%); border-bottom: 1px solid color-mix(in oklab, var(--muted), transparent 70%); z-index: 50; }
    nav { display: flex; align-items: center; justify-content: space-between; gap: 12px; }
    .brand { display: flex; align-items: center; gap: 10px; font-weight: 700; letter-spacing: .2px; }
    .brand .dot { width: 10px; height: 10px; border-radius: 999px; background: var(--brand); box-shadow: 0 0 0 3px var(--ring); }
    .navlinks a { margin-left: 16px; font-weight: 600; }
    .skip { position: absolute; left: -9999px; }
    .skip:focus { left: 12px; top: 12px; background: var(--brand); color: #fff; padding: 8px 12px; border-radius: 10px; }

    .hero { display: grid; grid-template-columns: 120px 1fr; gap: 20px; align-items: center; padding: 36px 0 12px; }
    .hero img { width: 120px; height: 120px; border-radius: 999px; object-fit: cover; border: 4px solid color-mix(in oklab, var(--brand), transparent 70%); box-shadow: 0 10px 30px color-mix(in oklab, var(--brand), transparent 80%); }
    .tag { display: inline-block; font-size: 12px; padding: 3px 8px; border-radius: 999px; background: color-mix(in oklab, var(--brand), white 85%); color: var(--brand-dark); font-weight: 700; letter-spacing: .3px; }
    h1 { margin: 8px 0 6px; font-size: clamp(28px, 4.5vw, 42px); line-height: 1.15; }
    .subtitle { color: var(--muted); margin: 0 0 16px; font-size: 16px; }

    .buttons { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 8px; }
    .btn { display: inline-flex; align-items: center; gap: 8px; padding: 10px 14px; border-radius: 12px; border: 1px solid color-mix(in oklab, var(--brand), transparent 75%); background: linear-gradient(180deg, color-mix(in oklab, var(--card), white 8%), color-mix(in oklab, var(--card), black 8%)); color: var(--text); font-weight: 700; text-decoration: none; box-shadow: 0 8px 16px rgba(0,0,0,.05); transition: transform .05s ease, box-shadow .2s ease; }
    .btn:hover { transform: translateY(-1px); box-shadow: 0 10px 24px rgba(0,0,0,.08); text-decoration: none; }
    .btn.primary { background: linear-gradient(180deg, color-mix(in oklab, var(--brand), white 75%), var(--brand)); color: white; border-color: var(--brand-dark); }

    section { margin: 36px 0; }
    .card { background: var(--card); border: 1px solid color-mix(in oklab, var(--muted), transparent 80%); border-radius: 16px; padding: 18px; box-shadow: 0 10px 20px rgba(0,0,0,.05); }

    .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 18px; }
    .project { display: flex; flex-direction: column; gap: 10px; }
    .project h3 { margin: 0; }
    .project p { margin: 0; color: var(--muted); }
    .project .meta { font-size: 13px; color: var(--muted); }

    footer { margin: 48px 0 24px; color: var(--muted); font-size: 14px; display: flex; justify-content: space-between; flex-wrap: wrap; gap: 8px; }

    .sr-only { position: absolute; width: 1px; height: 1px; padding: 0; margin: -1px; overflow: hidden; clip: rect(0,0,0,0); white-space: nowrap; border: 0; }

    /* Simple responsive tweaks */
    @media (max-width: 540px){ .hero { grid-template-columns: 90px 1fr; } .hero img { width: 90px; height: 90px; } }
  </style>
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Person",
    "name": "Your Name",
    "url": "https://your-username.github.io/",
    "image": "photo.jpg",
    "sameAs": ["https://www.linkedin.com/in/your-handle", "https://github.com/your-username"],
    "jobTitle": "Your Role",
    "worksFor": { "@type": "Organization", "name": "Your School or Company" }
  }
  </script>
</head>
<body>
  <a class="skip" href="#main">Skip to content</a>
  <header>
    <div class="container">
      <nav aria-label="Primary">
        <div class="brand" aria-label="Home">
          <span class="dot" aria-hidden="true"></span>
        </div>
        <div class="navlinks" role="navigation">
          <a href="#about">About</a>
          <a href="#projects">Projects</a>
          <a href="#contact">Contact</a>
        </div>
      </nav>
    </div>
  </header>

  <main id="main" class="container" tabindex="-1">
    <!-- HERO / INTRO -->
    <section aria-labelledby="intro-heading">
      <div class="hero">
        <!-- Replace photo.jpg with your image file name in the repo root -->
        <img src="1755101710952.jpg" alt="Portrait of Your Name" />
        <div>
          <h1 id="intro-heading">Hi, I’m <span style="color:var(--brand)">Dereck Taverne</span>.</h1>
          <p class="subtitle">Welcome to my personal portfolio website!</p>
          <div class="buttons">
            <!-- Replace resume.pdf with your file name -->
            <a class="btn primary" href="resume.pdf" target="_blank" rel="noopener" aria-label="Open resume in new tab">📄 View Resume</a>
            <a class="btn" href="https://www.linkedin.com/in/dereck-taverne" target="_blank" rel="noopener" aria-label="LinkedIn profile">🔗 LinkedIn</a>
            <a class="btn" href="https://github.com/dereckTav" target="_blank" rel="noopener" aria-label="GitHub profile">💻 GitHub</a>
          </div>
        </div>
      </div>
      <div id="about" class="card" style="margin-top:12px">
        <h2>About</h2>
        <p>
          I’m a Computer Science major at Baruch College passionate about building efficient, data-driven backend systems, with experience in Java, Python, AWS, and projects ranging from multithreaded crawlers to AI/ML models.
        </p>
        <p><strong>Fun fact:</strong> I enjoy boxing in my free time — it’s a great stress reliever and a lot of fun!
        </p>
      </div>
    </section>
    
    <!--
    <!-- PROJECTS -->
    <!-- <section id="projects" aria-labelledby="projects-heading">
    <!--  <h2 id="projects-heading">Projects</h2>
    <!--  <div class="grid">
    <!--    <!-- Project Card 1 -->
    <!--    <article class="card project">
    <!--      <div>
    <!--        <h3><a href="https://github.com/your-username/project-one" target="_blank" rel="noopener">Project One</a></h3>
    <!--        <p>1–2 line description of what it does, the stack, and your role.</p>
    <!--      </div><!--
          <div clas<!--s="meta">Tech: Python, FastAPI • Highlights: Deployed on Render</div>
        </article>
        <!-- Project Card 2 -->
    <!--    <article class="card project">
          <div<!-->
    <!--        <h3><a href="https://github.com/your-username/project-two" target="_blank" rel=<!--"noopener">Project Two</a></h3>
    <!--        <p>1–2 line description of what it does, the stack, and your role.</p>
          </div<!-->
    <!--      <div class="meta">Tech: Java, Spring Boot • Highlights: 500+ users</div>
        </article><!--
        <!-- Project Card 3 -->
    <!--  <article class="card project">
    <!--      <div>
    <!--        <h3><a href="https://github.com/your-username/project-three" target="_blank" rel="noopener">Project Three</a></h3>
    <!--        <p>1–2 line description of what it does, the stack, and your role.</p>
    <!--      </div>
    <!--      <div class="meta">Tech: JavaScript, React • Highlights: Lighthouse 95+</div>
    <!--    </article>
    <!--  </div>
    <!-- </section>
    -->

    <!-- CONTACT / LINKS -->
    <section id="contact" aria-labelledby="contact-heading">
      <h2 id="contact-heading">Contact</h2>
      <div class="card">
        <p>Best way to reach me:</p>
        <ul>
          <li>Email: <a href="mailto:derecktaverne@gmail.com">derecktaverne@gmail.com</a></li>
          <li>LinkedIn: <a href="https://www.linkedin.com/in/dereck-taverne" target="_blank" rel="noopener">@Dereck Taverne</a></li>
          <li>GitHub: <a href="https://github.com/dereckTav" target="_blank" rel="noopener">@dereckTav</a></li>
        </ul>
      </div>
    </section>
  </main>

  <footer class="container" aria-label="Site footer">
    <div>© <span id="year"></span> Your Name</div>
    <div>
      <!-- Inline SVG icons so there are no external dependencies -->
      <a href="https://github.com/your-username" target="_blank" rel="noopener" aria-label="GitHub" title="GitHub" style="margin-right:10px"> 
        <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 .5A11.5 11.5 0 0 0 .5 12.3c0 5.2 3.4 9.6 8.2 11.2.6.1.8-.3.8-.6v-2c-3.3.7-4-1.4-4-1.4-.5-1.3-1.2-1.7-1.2-1.7-1-.7.1-.7.1-.7 1.2.1 1.8 1.2 1.8 1.2 1 .1.7 1.9 2.7 1.3.1-.8.4-1.3.8-1.6-2.7-.3-5.6-1.4-5.6-6a4.7 4.7 0 0 1 1.2-3.2 4.3 4.3 0 0 1 .1-3.2s1-.3 3.3 1.2a11.5 11.5 0 0 1 6 0c2.2-1.5 3.3-1.2 3.3-1.2a4.3 4.3 0 0 1 .1 3.2 4.7 4.7 0 0 1 1.2 3.2c0 4.6-2.9 5.6-5.6 5.9.5.4.9 1.1.9 2.3v3.4c0 .3.2.7.8.6 4.8-1.6 8.2-6 8.2-11.2A11.5 11.5 0 0 0 12 .5z"/></svg>
      </a>
      <a href="https://www.linkedin.com/in/your-handle" target="_blank" rel="noopener" aria-label="LinkedIn" title="LinkedIn">
        <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8.5h4V23h-4V8.5zm7.5 0h3.8v2h.1c.5-1 1.8-2.2 3.8-2.2 4 0 4.7 2.6 4.7 6V23h-4v-6.3c0-1.5 0-3.4-2.1-3.4s-2.4 1.6-2.4 3.3V23h-4V
