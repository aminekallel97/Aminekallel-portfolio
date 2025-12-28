# Aminekallel-portfolio
Amine's portfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Amine Kallel | Mechanical Engineer</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    * { box-sizing: border-box; scroll-behavior: smooth; }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #0f172a;
      color: #e5e7eb;
    }

    /* NAVBAR */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(15, 23, 42, 0.9);
      backdrop-filter: blur(10px);
      padding: 15px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
    }

    nav a {
      color: #e5e7eb;
      margin-left: 25px;
      text-decoration: none;
      font-weight: 400;
      font-size: 14px;
    }

    nav a:hover { color: #38bdf8; }

    /* HERO */
    header {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }

    header h1 {
      font-size: 48px;
      margin-bottom: 10px;
    }

    header p {
      font-size: 18px;
      color: #94a3b8;
    }

    /* SECTIONS */
    section {
      max-width: 900px;
      margin: auto;
      padding: 100px 20px;
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.8s ease;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    h2 {
      font-size: 28px;
      margin-bottom: 20px;
      color: #38bdf8;
    }

    /* SKILLS */
    .skills span {
      display: inline-block;
      background: #1e293b;
      padding: 8px 14px;
      margin: 6px;
      border-radius: 20px;
      font-size: 13px;
    }

    /* EXPERIENCE */
    .item {
      margin-bottom: 25px;
    }

    .item h3 { margin-bottom: 5px; }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 40px 20px;
      color: #94a3b8;
      font-size: 14px;
    }

    footer a { color: #38bdf8; text-decoration: none; }

    @media (max-width: 768px) {
      header h1 { font-size: 36px; }
      nav { padding: 15px 20px; }
    }
  </style>
</head>
<body>

<nav>
  <strong>AK</strong>
  <div>
    <a href="#about">About</a>
    <a href="#work">Current Work</a>
    <a href="#skills">Skills</a>
    <a href="#experience">Experience</a>
    <a href="#contact">Contact</a>
  </div>
</nav>

<header>
  <h1>Amine Kallel</h1>
  <p>Mechanical Engineer · Design · Industrial Optimization</p>
  <div style="margin-top:20px;">
    <a href="CV-Amine-Kallel.pdf" style="padding:10px 18px;border:1px solid #38bdf8;border-radius:25px;color:#38bdf8;text-decoration:none;font-size:14px;">Download CV</a>
  </div>
</header>

<section id="about">
  <h2>About Me</h2>
  <p>
    Mechanical engineer specialized in industrial process optimization, machine design and technical project management.
    Experienced in production, quality and engineering design, with a strong focus on continuous improvement and innovation.
  </p>
</section>

<section id="work">
  <h2>Current Focus</h2>
  <ul>
    <li>3D CAD design of custom rotating machines</li>
    <li>Technical solution development based on client needs</li>
    <li>Cost reduction and assembly optimization</li>
    <li>Technical mentoring within the design office</li>
  </ul>
</section>

<section id="skills">
  <h2>Skills & Tools</h2>
  <div class="skills">
    <span>SolidWorks</span><span>CATIA V5</span><span>AutoCAD</span>
    <span>AMDEC</span><span>8D</span><span>QRQC</span>
    <span>Six Sigma</span><span>SimaPro</span><span>OpenLCA</span>
    <span>Project Management</span><span>Leadership</span>
  </div>
</section>

<section id="projects">
  <h2>Projects</h2>

  <div class="item">
    <h3>Custom Rotating Machine Design</h3>
    <p>Design and 3D modeling of customized industrial machines using SolidWorks. Focus on manufacturability, weight optimization and cost reduction.</p>
  </div>

  <div class="item">
    <h3>Production Line Optimization</h3>
    <p>Improved assembly line efficiency from 74% to 85% through process analysis, KPI monitoring (OEE/TRS) and continuous improvement actions.</p>
  </div>

  <div class="item">
    <h3>Customer Quality Improvement</h3>
    <p>Management of customer complaints using 8D, AMDEC and QRQC methodologies, significantly reducing recurring defects.</p>
  </div>
</section>

<section id="experience">
  <h2>Experience</h2>

  <div class="item">
    <h3>Design Engineer – TUNICAD</h3>
    <p>2025 – Present · Sousse</p>
  </div>

  <div class="item">
    <h3>Customer Quality Engineer – PROMENS</h3>
    <p>2025 · Monastir</p>
  </div>

  <div class="item">
    <h3>Assembly Production Manager – PROMENS</h3>
    <p>2024 · Monastir</p>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>
    📧 <a href="mailto:kallelamine@outlook.com">kallelamine@outlook.com</a><br />
    🔗 <a href="https://linkedin.com/in/aminekallel" target="_blank">LinkedIn</a>
  </p>
</section>

<footer>
  © 2025 · Amine Kallel
</footer>

<script>
  const sections = document.querySelectorAll('section');

  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  }, { threshold: 0.15 });

  sections.forEach(section => observer.observe(section));
</script>

</body>
</html>
