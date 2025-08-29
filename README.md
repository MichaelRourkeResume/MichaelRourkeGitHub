<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title> Michael Rourke | Aerospace Engineering Professional</title>
  <!-- Enhanced SEO and Social Media -->
  <link rel="icon" type="image/jpg" href="Michael web site/assets/Switchboard.jpg">
  <meta name="description" content="Aerospace Engineering professional specializing in propulsion systems, vehicle dynamics, and advanced manufacturing. Experience in thermodynamics research, rocket design, and electrical systems.">
  <meta name="keywords" content="aerospace engineer, propulsion systems, rocket design, CAD, MATLAB, thermodynamics, Notre Dame">
  <meta property="og:title" content="Michael Rourke | Aerospace Engineering Professional">
  <meta property="og:description" content="Specializing in propulsion systems, vehicle dynamics, and advanced manufacturing technologies.">
  <meta property="og:image" content="assets/images/hero.jpg">
  <meta name="theme-color" content="#1a365d">

  <!-- Modern Typography -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  
  <style>
    :root {
      --primary: #1a365d;
      --primary-light: #2d5a87;
      --accent: #3182ce;
      --accent-light: #63b3ed;
      --success: #38a169;
      --bg: #f7fafc;
      --bg-secondary: #edf2f7;
      --text-primary: #1a202c;
      --text-secondary: #4a5568;
      --text-muted: #718096;
      --white: #ffffff;
      --border: #e2e8f0;
      --shadow-sm: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06);
      --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
      --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
      --shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
      --radius: 12px;
      --radius-lg: 16px;
      --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      color: var(--text-primary);
      background: var(--bg);
      line-height: 1.6;
      font-weight: 400;
    }

    /* Enhanced Typography */
    h1 { font-size: 3rem; font-weight: 800; line-height: 1.1; }
    h2 { font-size: 2rem; font-weight: 700; line-height: 1.2; }
    h3 { font-size: 1.5rem; font-weight: 600; line-height: 1.3; }
    h4 { font-size: 1.25rem; font-weight: 600; }
    p { font-size: 1rem; line-height: 1.7; }
    
    @media (max-width: 768px) {
      h1 { font-size: 2.25rem; }
      h2 { font-size: 1.75rem; }
      h3 { font-size: 1.25rem; }
    }

    /* Navigation */
    .navbar {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 100;
      background: rgba(255, 255, 255, 0.95);
      backdrop-filter: blur(20px);
      border-bottom: 1px solid var(--border);
      transition: var(--transition);
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-weight: 800;
      font-size: 1.5rem;
      color: var(--primary);
      text-decoration: none;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    .nav-links a {
      color: var(--text-secondary);
      text-decoration: none;
      font-weight: 500;
      padding: 0.5rem 1rem;
      border-radius: var(--radius);
      transition: var(--transition);
    }

    .nav-links a:hover {
      color: var(--primary);
      background: var(--bg-secondary);
    }

    /* Mobile Menu */
    .mobile-menu-btn {
      display: none;
      background: none;
      border: none;
      font-size: 1.5rem;
      color: var(--primary);
      cursor: pointer;
    }

    @media (max-width: 768px) {
      .nav-links {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: var(--white);
        flex-direction: column;
        padding: 1rem;
        box-shadow: var(--shadow-lg);
      }

      .nav-links.active {
        display: flex;
      }

      .mobile-menu-btn {
        display: block;
      }
    }

    /* Container */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    .section {
      padding: 6rem 0;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
      color: var(--white);
      padding: 8rem 0 6rem;
      margin-top: 80px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="50" cy="50" r="2" fill="rgba(255,255,255,0.1)"/></svg>') repeat;
      opacity: 0.3;
    }

    .hero-content {
      display: grid;
      grid-template-columns: 150px 1fr;
      gap: 3rem;
      align-items: center;
      position: relative;
      z-index: 1;
    }

    .hero-image {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid rgba(255, 255, 255, 0.3);
      box-shadow: var(--shadow-xl);
    }

    .hero-text h1 {
      margin-bottom: 1rem;
      background: linear-gradient(135deg, #ffffff 0%, #e2e8f0 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero-subtitle {
      font-size: 1.25rem;
      font-weight: 500;
      margin-bottom: 2rem;
      opacity: 0.9;
    }

    .hero-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-bottom: 3rem;
    }

    .tag {
      background: rgba(255, 255, 255, 0.15);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.2);
      color: var(--white);
      padding: 0.75rem 1.25rem;
      border-radius: 50px;
      font-weight: 500;
      font-size: 0.9rem;
    }

    .cta-buttons {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 1rem 2rem;
      border-radius: var(--radius);
      text-decoration: none;
      font-weight: 600;
      transition: var(--transition);
      cursor: pointer;
      border: none;
      font-size: 1rem;
    }

    .btn-primary {
      background: var(--white);
      color: var(--primary);
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: var(--shadow-lg);
    }

    .btn-secondary {
      background: transparent;
      color: var(--white);
      border: 2px solid rgba(255, 255, 255, 0.3);
    }

    .btn-secondary:hover {
      background: rgba(255, 255, 255, 0.1);
      border-color: rgba(255, 255, 255, 0.5);
    }

    @media (max-width: 768px) {
      .hero-content {
        grid-template-columns: 120px 1fr;
        gap: 2rem;
      }
      
      .hero-image {
        width: 120px;
        height: 120px;
      }
    }

    /* Cards */
    .card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow-sm);
      padding: 2rem;
      transition: var(--transition);
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: var(--shadow-lg);
    }

    /* About Section */
    .about-grid {
      display: grid;
      grid-template-columns: 2fr 1fr;
      gap: 3rem;
      margin-top: 3rem;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 1.5rem;
    }

    .stat-item {
      text-align: center;
      padding: 1.5rem;
      background: var(--bg-secondary);
      border-radius: var(--radius);
    }

    .stat-number {
      font-size: 2rem;
      font-weight: 800;
      color: var(--accent);
      display: block;
    }

    .stat-label {
      color: var(--text-muted);
      font-size: 0.9rem;
      font-weight: 500;
    }

    .skills-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
      margin-top: 1rem;
    }

    .skill-tag {
      background: var(--accent-light);
      color: var(--white);
      padding: 0.5rem 1rem;
      border-radius: 50px;
      font-size: 0.85rem;
      font-weight: 500;
    }

    @media (max-width: 768px) {
      .about-grid {
        grid-template-columns: 1fr;
      }
      
      .stats {
        grid-template-columns: 1fr;
      }
    }

    /* Experience Section */
    .experience-timeline {
      position: relative;
      margin-top: 3rem;
    }

    .experience-item {
      position: relative;
      margin-bottom: 3rem;
      padding-left: 3rem;
    }

    .experience-item::before {
      content: '';
      position: absolute;
      left: 0;
      top: 0.5rem;
      width: 1rem;
      height: 1rem;
      background: var(--accent);
      border-radius: 50%;
      border: 3px solid var(--white);
      box-shadow: 0 0 0 3px var(--accent-light);
    }

    .experience-item:not(:last-child)::after {
      content: '';
      position: absolute;
      left: 0.4rem;
      top: 1.5rem;
      width: 2px;
      height: calc(100% + 1rem);
      background: var(--border);
    }

    .experience-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 1rem;
    }

    .experience-title {
      color: var(--primary);
      margin-bottom: 0.5rem;
    }

    .experience-company {
      color: var(--text-secondary);
      font-weight: 500;
    }

    .experience-date {
      background: var(--bg-secondary);
      color: var(--text-muted);
      padding: 0.5rem 1rem;
      border-radius: var(--radius);
      font-size: 0.9rem;
      font-weight: 500;
      white-space: nowrap;
    }

    .experience-achievements {
      list-style: none;
      margin-top: 1rem;
    }

    .experience-achievements li {
      position: relative;
      padding-left: 1.5rem;
      margin-bottom: 0.75rem;
      color: var(--text-secondary);
    }

    .experience-achievements li::before {
      content: '▶';
      position: absolute;
      left: 0;
      color: var(--accent);
      font-size: 0.8rem;
    }

    /* Projects Grid */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
      gap: 2rem;
      margin-top: 3rem;
    }

    .project-card {
      overflow: hidden;
    }

    .project-image {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: var(--radius);
      margin-bottom: 1.5rem;
      transition: var(--transition);
    }

    .project-card:hover .project-image {
      transform: scale(1.05);
    }

    .project-title {
      color: var(--primary);
      margin-bottom: 1rem;
    }

    .project-description {
      color: var(--text-secondary);
      margin-bottom: 1.5rem;
    }

    .project-tech {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .tech-tag {
      background: var(--bg-secondary);
      color: var(--text-muted);
      padding: 0.25rem 0.75rem;
      border-radius: 50px;
      font-size: 0.8rem;
      font-weight: 500;
    }

    /* Contact Section */
    .contact {
      background: var(--bg-secondary);
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      margin-top: 3rem;
    }

    .contact-info {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 1rem;
      padding: 1rem;
      background: var(--white);
      border-radius: var(--radius);
      text-decoration: none;
      color: var(--text-primary);
      transition: var(--transition);
    }

    .contact-item:hover {
      transform: translateX(8px);
      box-shadow: var(--shadow-md);
    }

    .contact-icon {
      width: 24px;
      height: 24px;
      color: var(--accent);
    }

    .download-resume {
      background: var(--success);
      color: var(--white);
      padding: 1.5rem 2rem;
      border-radius: var(--radius);
      text-align: center;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.1rem;
      transition: var(--transition);
    }

    .download-resume:hover {
      background: #2f855a;
      transform: translateY(-2px);
      box-shadow: var(--shadow-lg);
    }

    @media (max-width: 768px) {
      .contact-grid {
        grid-template-columns: 1fr;
      }
      
      .experience-header {
        flex-direction: column;
        gap: 0.5rem;
      }
    }

    /* Footer */
    .footer {
      background: var(--primary);
      color: var(--white);
      text-align: center;
      padding: 3rem 0;
    }

    /* Animations */
    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .fade-in-up {
      animation: fadeInUp 0.8s ease-out forwards;
    }

    /* Section Headers */
    .section-header {
      text-align: center;
      margin-bottom: 3rem;
    }

    .section-title {
      color: var(--primary);
      margin-bottom: 1rem;
    }

    .section-subtitle {
      color: var(--text-muted);
      font-size: 1.1rem;
      max-width: 600px;
      margin: 0 auto;
    }
  </style>
</head>
<body>
  <!-- Navigation -->
  <nav class="navbar">
    <div class="nav-container">
      <a href="#" class="logo">MR</a>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <button class="mobile-menu-btn">☰</button>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <div class="container">
      <div class="hero-content">
        <img
          class="hero-image"
          src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Headshot.jpg"
          alt="Michael Rourke - Professional Headshot"
          loading="eager">
        <div class="hero-text">
          <h1>Michael Rourke</h1>
          <p class="hero-subtitle">Aerospace Engineering Senior | University of Notre Dame</p>
          <div class="hero-tags">
            <span class="tag">Propulsion Systems</span>
            <span class="tag">Vehicle Dynamics</span>
            <span class="tag">CAD & Manufacturing</span>
            <span class="tag">MATLAB Simulation</span>
          </div>
          <div class="cta-buttons">
            <a href="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Michael Rourke Resume 2025 v6 (1).pdf" class="btn btn-primary" download>
              📄 Download Resume
            </a>
            <a href="#contact" class="btn btn-secondary">
              💬 Get In Touch
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">About Me</h2>
        <p class="section-subtitle">Passionate aerospace engineer with expertise in propulsion systems, thermodynamics, and advanced manufacturing technologies.</p>
      </div>
      <div class="about-grid">
        <div class="card">
          <h3 style="color: var(--primary); margin-bottom: 1.5rem;">Professional Overview</h3>
          <p style="margin-bottom: 1.5rem;">I'm a dedicated Aerospace Engineering junior at the University of Notre Dame with hands-on experience in thermodynamic cycle modeling, propulsion system integration, and advanced CAD-based manufacturing design. My passion lies in solving complex engineering challenges through innovative design and rigorous analysis.</p>
          <p style="margin-bottom: 1.5rem;">My experience spans from competitive rocket design and thermodynamics research in Rome to electrical systems engineering at SAI Advanced Power Solutions. I bring a unique combination of theoretical knowledge and practical application to every project.</p>
          <h4 style="margin-bottom: 1rem;">Core Competencies</h4>
          <div class="skills-list">
            <span class="skill-tag">SolidWorks</span>
            <span class="skill-tag">Creo Parametric</span>
            <span class="skill-tag">Fusion 360</span>
            <span class="skill-tag">MATLAB/Simulink</span>
            <span class="skill-tag">RockSim</span>
            <span class="skill-tag">OpenRocket</span>
            <span class="skill-tag">Thermodynamics</span>
            <span class="skill-tag">Propulsion Design</span>
            <span class="skill-tag">3D Printing</span>
            <span class="skill-tag">Manufacturing</span>
          </div>
        </div>
        <div class="card">
          <h4 style="margin-bottom: 1rem;">Quick Facts</h4>
          <p><strong>📍 Location:</strong> Bartlett, IL</p>
          <p><strong>🎯 Focus Areas:</strong> Propulsion, Rocketry, Controls</p>
          <p><strong>🏫 University:</strong> Notre Dame (Junior)</p>
          <p><strong>🚀 Clubs:</strong> ND Rocketry Club, Fighting for St. Jude</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Experience Section -->
  <section id="experience" class="section" style="background: var(--bg-secondary);">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Professional Experience</h2>
        <p class="section-subtitle">A track record of innovation and excellence across aerospace and engineering disciplines.</p>
      </div>
      <div class="experience-timeline">
        <div class="experience-item">
          <div class="experience-header">
            <div>
              <h3 class="experience-title">Thermodynamics Research Assistant</h3>
              <p class="experience-company">Notre Dame Global Gateway - Rome, Italy</p>
            </div>
            <span class="experience-date">Aug 2024 – Dec 2024</span>
          </div>
          <ul class="experience-achievements">
            <li>Collaborated with Professor Pietro Paolo Ciottoli on cutting-edge thermodynamic cycle efficiency research for aerospace propulsion applications</li>
            <li>Developed comprehensive MATLAB simulation models for combustion dynamics and heat transfer analysis in advanced engine configurations</li>
            <li>Conducted parametric studies of Brayton cycle performance and created sophisticated visualization tools for data interpretation and research presentation</li>
            <li>Contributed to international aerospace research standards and methodologies</li>
          </ul>
        </div>
        <div class="experience-item">
          <div class="experience-header">
            <div>
              <h3 class="experience-title">Design Engineer</h3>
              <p class="experience-company">Notre Dame Rocketry Club</p>
            </div>
            <span class="experience-date">Aug 2023 – May 2024</span>
          </div>
          <ul class="experience-achievements">
            <li>Engineered propulsion integration systems using Fusion 360 for competition rocket achieving 4,000+ ft altitude with precision accuracy</li>
            <li>Selected and analyzed advanced composite materials to optimize thrust-to-weight ratio while maintaining structural integrity under extreme conditions</li>
            <li>Performed comprehensive aerodynamic simulations using RockSim and OpenRocket to ensure stable, predictable flight characteristics</li>
            <li>Led final assembly coordination of rocket components with high-precision alignment and secure mechanical connections</li>
          </ul>
        </div>
        <div class="experience-item">
          <div class="experience-header">
            <div>
              <h3 class="experience-title">Engineering Intern</h3>
              <p class="experience-company">SAI Advanced Power Solutions</p>
            </div>
            <span class="experience-date">May 2023 – Jul 2025 (Multiple Terms)</span>
          </div>
          <ul class="experience-achievements">
            <li>Designed optimized component layouts for manufacturing systems using Creo CAD, improving production efficiency and reducing assembly time</li>
            <li>Executed comprehensive electrical testing protocols including Hypot, multimeter diagnostics, and 480V system verification for low/medium-voltage switchboards</li>
            <li>Spearheaded quality assurance initiatives in electrical system assembly, achieving zero-defect verification standards</li>
            <li><strong>Process Improvement:</strong> Developed improved insulation process for bus bar MCCB connectors using heat shrink tubing, reducing material costs by 25% while decreasing installation time significantly</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Featured Projects</h2>
        <p class="section-subtitle">Innovative engineering solutions showcasing technical expertise and creative problem-solving.</p>
      </div>
      <div class="projects-grid">
        <div class="card project-card">
          <img
            class="project-image"
            src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Catapult_pic.JPEG"
            alt="Award-winning mechanical catapult design"
            loading="lazy">
          <h3 class="project-title">🏆 Award-Winning Mechanical Catapult</h3>
          <p class="project-description">Designed and fabricated a 1st place competition catapult using advanced manufacturing techniques including 3D printing and precision water-jet cutting. Featured simulation-driven redesign of launcher arm and trigger mechanism for optimal range and reliability.</p>
          <div class="project-tech">
            <span class="tech-tag">SolidWorks</span>
            <span class="tech-tag">3D Printing</span>
            <span class="tech-tag">Water-Jet Cutting</span>
            <span class="tech-tag">Mechanical Design</span>
          </div>
        </div>
        <div class="card project-card">
          <img
            class="project-image"
            src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/RC_Car_Pic.png"
            alt="High-performance RC car drivetrain system"
            loading="lazy">
          <h3 class="project-title">🚗 High-Performance RC Car System</h3>
          <p class="project-description">Engineered award-winning drive system optimized for speed, torque, and ramp handling capabilities. Utilized SolidWorks motion simulation to optimize drivetrain performance and integrate defensive/projectile systems for competition scenarios.</p>
          <div class="project-tech">
            <span class="tech-tag">SolidWorks</span>
            <span class="tech-tag">Motion Simulation</span>
            <span class="tech-tag">Drivetrain Design</span>
            <span class="tech-tag">Systems Integration</span>
          </div>
        </div>
        <div class="card project-card">
          <img
            class="project-image"
            src="/workspaces/MichaelRourkeGitHub/Michael web site/assets/BraytonPic.png"
            alt="Advanced vehicle dynamics simulation interface"
            loading="lazy">
          <h3 class="project-title">🔬 Vehicle Systems Simulation</h3>
          <p class="project-description">Developed comprehensive MATLAB-based model simulating complex vehicle dynamics with environmental variability factors. Created multi-DOF framework enabling real-time system response analysis for aerospace applications.</p>
          <div class="project-tech">
            <span class="tech-tag">MATLAB</span>
            <span class="tech-tag">Simulink</span>
            <span class="tech-tag">Systems Modeling</span>
            <span class="tech-tag">Data Visualization</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section contact">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Let's Connect</h2>
        <p class="section-subtitle">Ready to discuss opportunities in aerospace engineering, propulsion systems, or innovative engineering solutions.</p>
      </div>
      <div class="contact-grid">
        <div class="contact-info">
          <a href="mailto:mrourke@nd.edu" class="contact-item">
            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
              <path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.89 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
            </svg>
            <div>
              <strong>Email</strong>
              <p>mrourke@nd.edu</p>
            </div>
          </a>
          <a href="tel:+13317030556" class="contact-item">
            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
              <path d="M6.62 10.79c1.44 2.83 3.76 5.14 6.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24 1.12.37 2.33.57 3.57.57.55 0 1 .45 1 1V20c0 .55-.45 1-1 1-9.39 0-17-7.61-17-17 0-.55.45-1 1-1h3.5c.55 0 1 .45 1 1 0 1.25.2 2.45.57 3.57.11.35.03.74-.25 1.02l-2.2 2.2z"/>
            </svg>
            <div>
              <strong>Phone</strong>
              <p>(331) 703-0556</p>
            </div>
          </a>
          <a href="https://www.linkedin.com/in/michael-rourke-39508625a/" target="_blank" rel="noopener" class="contact-item">
            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
              <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
            </svg>
            <div>
              <strong>LinkedIn</strong>
              <p>Connect with me professionally</p>
            </div>
          </a>
          <div class="contact-item" style="background: var(--bg-secondary); cursor: default;">
            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
              <path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/>
            </svg>
            <div>
              <strong>Location</strong>
              <p>Bartlett, IL | Open to Relocation</p>
            </div>
          </div>
        </div>
        <div>
          <a href="/workspaces/MichaelRourkeGitHub/Michael web site/assets/Michael Rourke Resume 2025 v6 (1).pdf" download class="download-resume">
            <svg style="width: 24px; height: 24px; margin-right: 0.5rem;" fill="currentColor" viewBox="0 0 24 24">
              <path d="M14,2H6A2,2 0 0,0 4,4V20A2,2 0 0,0 6,22H18A2,2 0 0,0 20,20V8L14,2M18,20H6V4H13V9H18V20Z"/>
            </svg>
            Download Complete Resume
          </a>
          <div class="card" style="margin-top: 2rem;">
            <h4 style="margin-bottom: 1rem; color: var(--primary);">🎯 Seeking Opportunities In:</h4>
            <ul style="list-style: none; padding: 0; margin: 0;">
              <li style="padding: 0.5rem 0; border-bottom: 1px solid var(--border);">✈️ Aerospace & Defense</li>
              <li style="padding: 0.5rem 0; border-bottom: 1px solid var(--border);">🚀 Propulsion Systems</li>
              <li style="padding: 0.5rem 0; border-bottom: 1px solid var(--border);">🔧 R&D Engineering</li>
              <li style="padding: 0.5rem 0; border-bottom: 1px solid var(--border);">📊 Systems Analysis</li>
              <li style="padding: 0.5rem 0;">🏭 Manufacturing Engineering</li>
            </ul>
          </div>
          <div class="card" style="margin-top: 2rem; background: linear-gradient(135deg, var(--accent-light), var(--accent)); color: white;">
            <h4 style="margin-bottom: 1rem; color: white;">🌟 What Sets Me Apart</h4>
            <ul style="list-style: none; padding: 0; margin: 0; color: rgba(255,255,255,0.9);">
              <li style="padding: 0.5rem 0;">• International research experience in Rome</li>
              <li style="padding: 0.5rem 0;">• Proven cost reduction achievements (25%)</li>
              <li style="padding: 0.5rem 0;">• Award-winning design competitions</li>
              <li style="padding: 0.5rem 0;">• Real-world industry internship experience</li>
              <li style="padding: 0.5rem 0;">• Strong technical and leadership skills</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="container">
      <p style="margin-bottom: 1rem;">&copy; 2025 Michael Rourke | Aerospace Engineering Professional</p>
      <p style="color: rgba(255,255,255,0.7); font-size: 0.9rem;">
        Passionate about pushing the boundaries of aerospace technology and engineering excellence.
      </p>
    </div>
  </footer>

  <!-- JavaScript for Mobile Menu -->
  <script>
    // Mobile menu toggle
    document.querySelector('.mobile-menu-btn').addEventListener('click', function() {
      document.querySelector('.nav-links').classList.toggle('active');
    });

    // Smooth scrolling for navigation links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          target.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
          });
        }
        // Close mobile menu after clicking
        document.querySelector('.nav-links').classList.remove('active');
      });
    });

    // Add scroll effect to navbar
    window.addEventListener('scroll', function() {
      const navbar = document.querySelector('.navbar');
      if (window.scrollY > 100) {
        navbar.style.background = 'rgba(255, 255, 255, 0.98)';
        navbar.style.boxShadow = '0 2px 20px rgba(0, 0, 0, 0.1)';
      } else {
        navbar.style.background = 'rgba(255, 255, 255, 0.95)';
        navbar.style.boxShadow = 'none';
      }
    });

    // Intersection Observer for animations
    const observerOptions = {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px'
    };

    const observer = new IntersectionObserver(function(entries) {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, observerOptions);

    // Observe cards and sections for animation
    document.querySelectorAll('.card, .experience-item, .section-header').forEach(el => {
      el.style.opacity = '0';
      el.style.transform = 'translateY(30px)';
      el.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
      observer.observe(el);
    });

    // Add loading animation for hero section
    window.addEventListener('load', function() {
      document.querySelector('.hero-content').style.animation = 'fadeInUp 1s ease-out forwards';
    });
  </script>

</body>
</html>
