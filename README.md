<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Michael Rourke | Aerospace Engineering</title>

  <!-- Favicon + Social preview (update paths) -->
  <link rel="icon" type="image/jpg" href="Michael web site/assets/Switchboard.jpg">
  <meta name="description" content="Aerospace Engineering at the University of Notre Dame focused on propulsion, vehicle dynamics, and hands-on engineering.">
  <meta property="og:title" content="Michael Rourke | Aerospace Engineering">
  <meta property="og:description" content="Propulsion, vehicle dynamics, and hands-on engineering.">
  <meta property="og:image" content="assets/images/hero.jpg">
  <meta name="theme-color" content="#0b3a6f">

  <style>
    :root{
      --bg:#f7f8fb;
      --text:#203040;
      --muted:#5a6b80;
      --brand:#0b5bd3;
      --brand-700:#0b3a6f;
      --card:#ffffff;
      --line:#e7ebf3;
      --shadow:0 6px 24px rgba(16,40,85,.08);
      --radius:16px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body {
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      color: var(--text);
      background: var(--bg);
      line-height: 1.6;
    }
    a { color: var(--brand); text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* Container */
    .wrap { max-width: 1080px; margin: 0 auto; padding: 24px; }

    /* Top nav */
    header.site {
      display:flex; align-items:center; justify-content:space-between;
      padding: 12px 0 8px; position: sticky; top: 0; background: rgba(247,248,251,.8);
      backdrop-filter: blur(8px); z-index: 50; border-bottom:1px solid var(--line);
    }
    .brand { font-weight: 800; letter-spacing:.3px; color: var(--brand-700); }
    nav a { margin-left: 18px; font-weight: 600; }

    /* Hero */
    .hero {
      margin-top: 16px; border-radius: var(--radius); overflow: hidden; position: relative;
      min-height: 280px; background: #0b3a6f url('assets/images/hero.jpg') center/cover no-repeat;
      box-shadow: var(--shadow);
    }
    .hero::after{
      content:""; position:absolute; inset:0; background: linear-gradient(180deg, rgba(5,20,45,.45), rgba(5,20,45,.65));
    }
    .hero-content{
      position: relative; z-index: 1; color: #fff; padding: 48px 32px;
      display: grid; grid-template-columns: 120px 1fr; gap: 20px; align-items: center;
    }
    .headshot{
      width:120px; height:120px; border-radius: 50%; object-fit: cover; border:3px solid rgba(255,255,255,.8);
    }
    .hero h1{ margin:0 0 6px; font-size: clamp(24px, 3.6vw, 40px); line-height:1.15;}
    .subtitle{ margin:0 0 12px; color:#e7eefb; font-weight:500; }
    .tags{ display:flex; flex-wrap:wrap; gap:8px; margin-top:8px;}
    .tag{ background: rgba(255,255,255,.14); border:1px solid rgba(255,255,255,.3); color:#fff; padding:6px 10px; border-radius:999px; font-size:.9rem;}

    /* Section */
    section { margin: 40px 0; }
    section h2 { color: var(--brand-700); margin-bottom: 12px; }
    .card{
      background: var(--card); border:1px solid var(--line); border-radius: var(--radius);
      box-shadow: var(--shadow); padding: 20px;
    }

    /* About layout */
    .about-grid{
      display:grid; grid-template-columns: 1.2fr .8fr; gap:24px;
    }
    .quick-list{margin:0;padding:0; list-style:none}
    .quick-list li{padding:8px 0; border-bottom:1px dashed var(--line)}
    .quick-list li:last-child{border-bottom:0}

    /* Project cards */
    .grid{
      display:grid; gap: 18px;
      grid-template-columns: repeat(12, 1fr);
    }
    .col-6{ grid-column: span 6; }
    .col-4{ grid-column: span 4; }
    @media (max-width: 860px){
      .about-grid{grid-template-columns: 1fr;}
      .col-6, .col-4{ grid-column: 1/-1; }
      .hero-content{ grid-template-columns: 88px 1fr; }
      .headshot{ width:88px; height:88px;}
    }

    .project{
      display:flex; flex-direction:column; gap:10px;
    }
    .project img{
      width:100%; height:220px; object-fit:cover; border-radius:12px; border:1px solid var(--line);
      background:#eef3fb;
    }
    .project h3{ margin:2px 0 0; }
    .meta{ color: var(--muted); font-size:.95rem; margin: -2px 0 6px; }
    .bullets{ margin:0; padding-left: 18px; }

    /* Gallery */
    .gallery{
      display:grid; gap:10px;
      grid-template-columns: repeat(6, 1fr);
    }
    .gallery img{
      width:100%; height:120px; object-fit:cover; border-radius:10px; border:1px solid var(--line);
      background:#eef3fb;
    }
    @media (max-width: 640px){
      .gallery{ grid-template-columns: repeat(3, 1fr); }
    }

    /* Contact */
    .buttons{ display:flex; flex-wrap:wrap; gap:10px; }
    .btn{
      display:inline-block; padding:10px 14px; border-radius:10px; border:1px solid var(--line);
      background:#fff; font-weight:600;
    }
    .btn.primary{ background: var(--brand); color:#fff; border-color: transparent; }
    .btn:hover{ transform: translateY(-1px); box-shadow: var(--shadow); text-decoration:none; }

    footer{
      text-align:center; padding: 28px 0 44px; color: var(--muted);
    }
  </style>
</head>
<body>

  <!-- Top navigation -->
  <div class="wrap">
    <header class="site">
      <div class="brand">MR</div>
      <nav>
        <a href="#about">About</a>
        <a href="#experience">Experience</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>
  </div>

  <!-- Hero -->
  <section class="wrap">
    <div class="hero" role="img" aria-label="Blue aerospace background image">
      <div class="hero-content">
        <!-- Headshot -->
        <img
          class="headshot"
          src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Headshot.jpg"
          alt="Portrait of Michael Rourke"
          width="240" height="240" loading="eager" decoding="async">
        <div>
          <h1>Michael Rourke</h1>
          <p class="subtitle">Aerospace Engineering Student · University of Notre Dame</p>
          <div class="tags">
            <span class="tag">Propulsion</span>
            <span class="tag">Vehicle Dynamics</span>
            <span class="tag">CAD &amp; Manufacturing</span>
            <span class="tag">MATLAB Simulation</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="wrap">
    <h2>About Me</h2>
    <div class="about-grid">
      <div class="card">
        <p>I’m a junior at the University of Notre Dame studying Aerospace Engineering. I’ve worked on thermodynamic cycle modeling, propulsion integration, CAD-based manufacturing design, and electronic testing of power systems. I'm passionate about propulsion, vehicle dynamics, and hands-on engineering challenges, and I'm actively seeking opportunities in aerospace systems and research.</p>
      </div>
      <!-- Quick facts card -->
      <aside class="card">
        <h3 style="margin-top:0;">Quick Facts</h3>
        <ul class="quick-list">
          <li><strong>Location:</strong> Bartlett, IL</li>
          <li><strong>Interests:</strong> Propulsion · Rocketry · Controls</li>
          <li><strong>Tools:</strong> SolidWorks, Creo, Fusion 360, MATLAB</li>
          <li><strong>Clubs:</strong> Notre Dame Rocketry Club, Notre Dame Fighting for St. Jude</li>
        </ul>
      </aside>
    </div>
  </section>

  <!-- Experience -->
  <section id="experience" class="wrap">
    <h2>Experience</h2>
    <div class="grid">
      <!-- Rocketry Club (with gallery) -->
      <div class="col-6 card">
        <div class="project">
          <img
            src="/workspaces/MichaelRourkeGitHub/Michael web site/Rocket_pic.png"
            alt="Competition rocket on launch rail"
            width="1200" height="700" loading="lazy" decoding="async">
          <h3>Notre Dame Rocketry Club – Design Engineer</h3>
          <div class="meta">Aug 2023 – May 2024</div>
          <ul class="bullets">
            <li>Designed propulsion integration systems in Fusion 360 for a competition rocket exceeding 4,000 ft altitude.</li>
            <li>Selected and analyzed composite materials to optimize thrust-to-weight ratio and structural integrity.</li>
            <li>Performed aerodynamic simulations using RockSim and Open Rocket to ensure stable, predictable flight.</li>
            <li>Led final assembly of rocket components with high-precision alignment and secure connections.</li>
          </ul>
          </div>
        </div>
      </div>
      <!-- Thermo Research -->
      <div class="col-6 card">
        <div class="project">
          <img
            src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/BraytonPic.png"
            alt="Thermodynamic cycle plot visualization"
            width="700" height="700" loading="lazy" decoding="async">
          <h3>Thermodynamics Research – Notre Dame Global Gateway (Rome)</h3>
          <div class="meta">Aug 2024 – Dec 2024</div>
          <ul class="bullets">
            <li>Assisted Professor Pietro Paolo Ciottoli on thermodynamic cycle efficiency for aerospace propulsion.</li>
            <li>Built MATLAB simulations for combustion dynamics and heat transfer in engine configurations.</li>
            <li>Conducted Brayton cycle parametric studies and created visualization tools for interpretation.</li>
          </ul>
        </div>
      </div>
      <!-- SAI Internship -->
      <div class="col-6 card">
        <div class="project">
          <img
            src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Switchboard.jpg"
            alt="Electrical testing setup at bench"
            width="1200" height="700" loading="lazy" decoding="async">
          <h3>SAI Advanced Power Solutions – Engineering Intern</h3>
          <div class="meta">May 2023 – Jul 2023, May 2024 – Jul 2024, May 2025 – Jul 2025</div>
          <ul class="bullets">
            <li>Used Creo CAD to design optimized component layouts for manufacturing systems.</li>
            <li>Performed Hypot, multimeter, and 480V system testing of low/medium-voltage switchboards.</li>
            <li>Led quality assurance in assembly of electrical systems for zero-defect verification.</li>
            <li>Developed innovative insulation process for bus bar MCCB connectors using heat shrink tubing, reducing material costs by 25% while decreasing installation time</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="projects" class="wrap">
    <h2>Projects</h2>
    <div class="grid">
      <!-- Mechanical Catapult -->
      <article class="col-4 card project">
        <img
          src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Catapult_pic.JPEG"
          alt="Compact 3D-printed mechanical catapult"
          width="800" height="500" loading="lazy" decoding="async">
        <h3>Mechanical Catapult</h3>
        <ul class="bullets">
          <li>Designed and fabricated 1st place catapult using 3D printing, and water-jet cutting.</li>
          <li>Simulation-driven redesign of launcher arm and trigger mechanism for range/reliability.</li>
        </ul>
      </article>
      <!-- RC Car System -->
      <article class="col-4 card project">
        <img
          src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/RC_Car_Pic.png"
          alt="RC car drivetrain assembly on bench"
          width="800" height="500" loading="lazy" decoding="async">
        <h3>RC Car System</h3>
        <ul class="bullets">
          <li>Built award winning drive system for speed, torque, and ramp handling.</li>
          <li>SolidWorks motion simulation to optimize drivetrain and integrate defense/projectile systems.</li>
        </ul>
      </article>
      <!-- Vehicle Systems Simulation -->
      <article class="col-4 card project">
        <img
          src="assets/images/vehiclesim.jpg"
          alt="Vehicle dynamics simulation chart"
          width="800" height="500" loading="lazy" decoding="async">
        <h3>Vehicle Systems Simulation</h3>
        <ul class="bullets">
          <li>MATLAB-based model simulating vehicle dynamics with environmental variability.</li>
          <li>Multi-DOF framework for real-time system response analysis.</li>
        </ul>
      </article>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="wrap">
    <h2>Contact</h2>
    <div class="card">
      <p><strong>Email:</strong> <a href="mailto:mrourke@nd.edu">mrourke@nd.edu</a></p>
      <p><strong>Phone:</strong> (331) 703-0556</p>
      <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/michael-rourke-39508625a/" target="_blank" rel="noopener">linkedin.com/in/michael-rourke-39508625a</a></p>
      <div class="buttons" style="margin-top:12px;">
        <!-- Point this to your resume PDF in the repo -->
        <a class="btn primary" href="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Michael Rourke Resume 2025 v6 (1).pdf" download>Download Resume (PDF)</a>
        <a class="btn" href="mailto:mrourke@nd.edu?subject=Interview%20Opportunity">Email Me</a>
      </div>
    </div>
  </section>

  <footer>
    <div class="wrap">
      © 2025 Michael Rourke
    </div>
  </footer>

</body>
</html>


