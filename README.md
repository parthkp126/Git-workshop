<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Parth Kaklotar — Portfolio</title>
  <meta name="description" content="Portfolio of Parth Kaklotar — Web Developer & Computer Engineering Student" />

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
  /* ==========================
     Professional White + Blue Portfolio
     Single-file (HTML + CSS + JS)
     Author: Generated for Parth Kaklotar
     ========================== */

  :root{
    --bg:#ffffff;
    --muted:#64748b;
    --text:#0f172a;
    --primary:#0ea5e9; /* blue */
    --primary-dark:#0369a1;
    --accent:#0b73c2;
    --card:#f8fafc;
    --glass: rgba(15,23,42,0.04);
    --radius:12px;
    --container:1200px;
    --ff: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    --transition: all 0.22s cubic-bezier(.4,0,.2,1);
  }

  *{box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{font-family:var(--ff);background:var(--bg);color:var(--text);line-height:1.6;margin:0;padding:0}

  .wrap{max-width:var(--container);margin:0 auto;padding:36px}

  /* NAV */
  .navbar{display:flex;align-items:center;justify-content:space-between;padding:18px 0}
  .brand{font-weight:800;font-size:1.25rem;background:linear-gradient(90deg,var(--primary),var(--accent));-webkit-background-clip:text;background-clip:text;color:transparent}
  .nav-links{display:flex;gap:10px}
  .nav-links a{padding:8px 12px;border-radius:8px;color:var(--text);text-decoration:none;font-weight:600;transition:var(--transition)}
  .nav-links a:hover{background:var(--card);color:var(--primary-dark)}

  /* Header / Hero */
  .hero{display:grid;grid-template-columns:260px 1fr;gap:36px;align-items:center;padding:40px 0}
  .hero-card{background:linear-gradient(180deg,#fff,#fbfdff);border-radius:var(--radius);box-shadow:0 8px 30px rgba(2,6,23,0.06);padding:22px;border:1px solid rgba(2,6,23,0.04)}
  .avatar{width:220px;height:220px;border-radius:14px;overflow:hidden;border:6px solid white;box-shadow:0 10px 30px rgba(3,105,161,0.08)}
  .avatar img{width:100%;height:100%;object-fit:cover;display:block}
  .hero-meta h1{margin:0;font-size:2rem;line-height:1.05}
  .hero-meta p.tag{color:var(--primary);font-weight:700;margin:10px 0}
  .intro{color:var(--muted);max-width:70ch}

  .hero-cta{margin-top:18px;display:flex;gap:12px;flex-wrap:wrap}
  .btn{display:inline-flex;align-items:center;gap:10px;padding:10px 16px;border-radius:10px;font-weight:700;border:none;cursor:pointer;transition:var(--transition)}
  .btn-primary{background:linear-gradient(90deg,var(--primary),var(--accent));color:white;box-shadow:0 8px 24px rgba(14,165,233,0.18)}
  .btn-outline{background:transparent;border:2px solid var(--primary);color:var(--primary)}

  /* Sections */
  section{padding:44px 0}
  h2.section-title{text-align:left;font-size:1.6rem;margin:0 0 18px;font-weight:800}
  .section-sub{color:var(--muted);margin-bottom:16px}

  .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:18px}
  .card{background:var(--card);border-radius:12px;padding:18px;border:1px solid rgba(2,6,23,0.04);box-shadow:0 6px 20px rgba(2,6,23,0.04);transition:var(--transition)}
  .card:hover{transform:translateY(-6px);box-shadow:0 12px 30px rgba(2,6,23,0.07)}
  .card h4{margin:0 0 8px;font-size:1.05rem}
  .card p{margin:0;color:var(--muted)}

  /* Projects: image part */
  .project-img{height:160px;border-radius:10px;overflow:hidden;margin-bottom:12px;background:linear-gradient(180deg,#e6f7ff,#f8fbff)}
  .project-img img{width:100%;height:100%;object-fit:cover;display:block}

  /* Contact */
  #contact .card{display:flex;align-items:center;gap:12px}
  .contact-icon{width:48px;height:48px;border-radius:10px;background:var(--glass);display:flex;align-items:center;justify-content:center;font-weight:800;color:var(--primary)}

  /* Footer */
  footer{border-top:1px solid rgba(2,6,23,0.04);padding:28px 0;margin-top:28px}
  .socials{display:flex;gap:10px}
  .socials a{padding:8px 12px;border-radius:10px;background:var(--card);text-decoration:none;color:var(--primary);font-weight:700}

  /* Responsive */
  @media (max-width:900px){
    .hero{grid-template-columns:1fr;text-align:center}
    .hero-card{margin-inline:auto}
    .avatar{width:180px;height:180px;border-radius:16px}
    .wrap{padding:22px}
  }

  /* Small utilities */
  .muted{color:var(--muted)}
  .small{font-size:0.9rem}
  .center{text-align:center}

  /* Simple reveal */
  .reveal{opacity:0;transform:translateY(12px);transition:all 0.6s cubic-bezier(.2,.8,.2,1)}
  .reveal.show{opacity:1;transform:none}

  </style>
</head>
<body>

  <div class="wrap">
    <nav class="navbar">
      <div class="brand">Parth Kaklotar</div>
      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#education">Education</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>

    <!-- HERO -->
    <header class="hero">
      <div class="hero-card avatar">
        <!-- Placeholder image -- replace profile.jpg in same folder -->
        <img src="profile.jpg" alt="Parth Kaklotar">
      </div>

      <div class="hero-meta">
        <h1>Parth Kaklotar</h1>
        <p class="tag">Computer Engineering Student • Web Developer</p>
        <p class="intro muted">I build clean, responsive websites and web apps. Currently pursuing a Diploma in Computer Engineering — passionate about front-end development, Google Workspace tools, and collaborating on real-world projects.</p>

        <div class="hero-cta">
          <a class="btn btn-primary" href="#contact">Contact Me</a>
          <a class="btn btn-outline" href="https://github.com/parthkp126" target="_blank">GitHub</a>
          <a class="btn btn-outline" href="resume.pdf" download>Download Resume</a>
        </div>

        <p class="small muted" style="margin-top:14px">Email: <a href="mailto:parthkaklotar544@gmail.com">parthkaklotar544@gmail.com</a></p>
      </div>
    </header>

    <!-- ABOUT -->
    <section id="about">
      <h2 class="section-title">About Me</h2>
      <p class="section-sub muted">I'm Parth — a motivated computer engineering student who loves building fast, user-friendly web experiences.</p>

      <div class="grid">
        <div class="card reveal">
          <h4>Passionate Learner</h4>
          <p>I keep learning modern web tools, participate in projects, and enjoy solving problems with code.</p>
        </div>

        <div class="card reveal">
          <h4>Team Player</h4>
          <p>I collaborate with classmates on projects and contribute to GitHub repositories.</p>
        </div>

        <div class="card reveal">
          <h4>Tools & Methods</h4>
          <p>Git, GitHub, Chrome DevTools, responsive design, semantic HTML, and accessibility-minded markup.</p>
        </div>
      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects">
      <h2 class="section-title">Projects</h2>
      <p class="section-sub muted">A few highlights — visit my GitHub for full code.</p>

      <div class="grid">
        <article class="card reveal">
          <div class="project-img"><img src="proj-portfolio.jpg" alt="Portfolio"></div>
          <h4>Personal Portfolio</h4>
          <p class="muted">A responsive portfolio showcasing projects, skills, and contact information. Built with semantic HTML, CSS, and lightweight JS.</p>
        </article>

        <article class="card reveal">
          <div class="project-img"><img src="proj-calculator.jpg" alt="Calculator"></div>
          <h4>Calculator App</h4>
          <p class="muted">A small JavaScript calculator focusing on clean UX and keyboard support.</p>
        </article>

        <article class="card reveal">
          <div class="project-img"><img src="proj-landing.jpg" alt="Landing"></div>
          <h4>Landing Page</h4>
          <p class="muted">A marketing-style landing page with responsive layout and subtle animations.</p>
        </article>
      </div>

    </section>

    <!-- SKILLS -->
    <section id="skills">
      <h2 class="section-title">Skills</h2>
      <p class="section-sub muted">Technologies and tools I use regularly.</p>

      <div class="grid">
        <div class="card reveal">
          <h4>Front-end</h4>
          <p class="muted">HTML5 • CSS3 • JavaScript • Responsive Design</p>
        </div>

        <div class="card reveal">
          <h4>Tools</h4>
          <p class="muted">Git • GitHub • VS Code • Chrome DevTools</p>
        </div>

        <div class="card reveal">
          <h4>Productivity</h4>
          <p class="muted">Google Workspace (Docs, Sheets, Slides, Drive)</p>
        </div>
      </div>
    </section>

    <!-- EDUCATION -->
    <section id="education">
      <h2 class="section-title">Education</h2>
      <div class="grid">
        <div class="card reveal">
          <h4>Diploma in Computer Engineering</h4>
          <p class="muted">Government Polytechnic College — 2023 – Present</p>
        </div>

        <div class="card reveal">
          <h4>10th Standard</h4>
          <p class="muted">GSEB Board — Completed</p>
        </div>
      </div>
    </section>

    <!-- CERTIFICATES -->
    <section id="certificates">
      <h2 class="section-title">Certificates</h2>
      <div class="grid">
        <div class="card reveal">
          <h4>Google Workspace Certification</h4>
          <p class="muted">Docs, Sheets, Slides, Drive — practical coursework.</p>
        </div>
        <div class="card reveal">
          <h4>Python Programming Basics</h4>
          <p class="muted">Introductory Python with small projects.</p>
        </div>
        <div class="card reveal">
          <h4>HTML & CSS Fundamentals</h4>
          <p class="muted">Front-end basics and practical exercises.</p>
        </div>
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="experience">
      <h2 class="section-title">Experience</h2>
      <div class="grid">
        <div class="card reveal">
          <h4>Web Development Intern</h4>
          <p class="muted">Worked on responsive pages using HTML/CSS/JS.</p>
        </div>
        <div class="card reveal">
          <h4>Team Project Collaborations</h4>
          <p class="muted">Built academic projects with classmates, using Git for version control.</p>
        </div>
      </div>
    </section>

    <!-- ACHIEVEMENTS -->
    <section id="achievements">
      <h2 class="section-title">Achievements</h2>
      <div class="grid">
        <div class="card reveal">
          <h4>Top 10 Rank</h4>
          <p class="muted">Strong academic performance in diploma semester exams.</p>
        </div>
        <div class="card reveal">
          <h4>Project Excellence Award</h4>
          <p class="muted">Recognized for an innovative mini-project in college.</p>
        </div>
      </div>
    </section>

    <!-- COURSES -->
    <section id="courses">
      <h2 class="section-title">Courses Completed</h2>
      <div class="grid">
        <div class="card reveal">
          <h4>Google Workspace Course</h4>
          <p class="muted">Docs, Sheets, Meet, Calendar, Drive.</p>
        </div>
        <div class="card reveal">
          <h4>Python Basics</h4>
          <p class="muted">Beginner-level Python programming.</p>
        </div>
        <div class="card reveal">
          <h4>HTML, CSS, JavaScript</h4>
          <p class="muted">Front-end fundamentals and projects.</p>
        </div>
      </div>
    </section>

    <!-- LANGUAGES -->
    <section id="languages">
      <h2 class="section-title">Languages Known</h2>
      <div class="grid">
        <div class="card reveal"><h4>English</h4><p class="muted">Good understanding, writing & speaking</p></div>
        <div class="card reveal"><h4>Gujarati</h4><p class="muted">Native</p></div>
        <div class="card reveal"><h4>Hindi</h4><p class="muted">Fluent</p></div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <h2 class="section-title">Contact</h2>
      <p class="section-sub muted">Feel free to reach out — available for internships and collaboration.</p>

      <div class="grid">
        <div class="card reveal">
          <div class="contact-icon">@</div>
          <div>
            <h4>Email</h4>
            <p class="muted"><a href="mailto:parthkaklotar544@gmail.com">parthkaklotar544@gmail.com</a></p>
          </div>
        </div>

        <div class="card reveal">
          <div class="contact-icon">GH</div>
          <div>
            <h4>GitHub</h4>
            <p class="muted"><a href="https://github.com/parthkp126" target="_blank">github.com/parthkp126</a></p>
          </div>
        </div>

        <div class="card reveal">
          <div class="contact-icon">in</div>
          <div>
            <h4>LinkedIn</h4>
            <p class="muted"><a href="https://www.linkedin.com/in/parth-kaklotar-39381a378?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">linkedin.com/in/parth-kaklotar</a></p>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer class="center">
      <div class="socials">
        <a href="https://github.com/parthkp126" target="_blank">GitHub</a>
        <a href="https://www.linkedin.com/in/parth-kaklotar-39381a378?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">LinkedIn</a>
        <a href="mailto:parthkaklotar544@gmail.com">Email</a>
      </div>
      <p class="small muted">© 2025 Parth Kaklotar • Built with care</p>
    </footer>

  </div>

  <script>
  // Simple reveal on scroll + basic nav active state
  (function(){
    const reveals = document.querySelectorAll('.reveal');
    function revealOnScroll(){
      const trigger = window.innerHeight * 0.85;
      reveals.forEach(el=>{
        const top = el.getBoundingClientRect().top;
        if(top < trigger) el.classList.add('show');
      });
    }
    revealOnScroll();
    window.addEventListener('scroll', revealOnScroll, {passive:true});

    // Smooth highlight for nav
    const navLinks = document.querySelectorAll('.nav-links a');
    function setActive(){
      const fromTop = window.scrollY + 80;
      navLinks.forEach(link=>{
        const section = document.querySelector(link.getAttribute('href'));
        if(!section) return;
        if(section.offsetTop <= fromTop && section.offsetTop + section.offsetHeight > fromTop){
          link.style.background = 'linear-gradient(90deg,var(--primary),var(--accent))';
          link.style.color = 'white';
        } else { link.style.background = 'transparent'; link.style.color = '' }
      })
    }
    setActive();
    window.addEventListener('scroll', setActive, {passive:true});

    // Mobile: simple nav toggle (if you add one later)
  })();
  </script>

</body>
</html>
