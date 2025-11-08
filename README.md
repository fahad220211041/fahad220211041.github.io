<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Md. Abdul Fahad - Final-year BBA student at BAUST seeking leadership internship opportunities. Experienced in business clubs, BNCC, and volunteering.">
  <title>My Design - Md. Abdul Fahad Portfolio</title>
  <script src="/_sdk/element_sdk.js"></script>
  <style>
        :root {
            --nav-height: 64px; /* adjust if you change nav padding/size */
            --accent-1: #0f172a;
            --accent-2: #1e3a8a;
            --accent-3: #3b82f6;
        }

        /* enable smooth scrolling for anchor links */
        html {
            scroll-behavior: smooth;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.7;
            color: #1e293b;
            background: linear-gradient(to bottom, #f8fafc 0%, #f1f5f9 100%);
            letter-spacing: -0.01em;
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
        }

        /* Top navigation (new) */
        .top-nav {
            position: sticky;
            top: 0;
            z-index: 1100;
            height: var(--nav-height);
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, var(--accent-1) 0%, var(--accent-2) 100%);
            box-shadow: 0 6px 20px rgba(2,6,23,0.12);
            padding: 0 1rem;
        }

        .nav-inner {
            width: 100%;
            max-width: 1200px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }

        .nav-links {
            display:flex;
            gap: 0.25rem;
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-links a {
            color: rgba(255,255,255,0.95);
            text-decoration: none;
            padding: 0.5rem 0.9rem;
            border-radius: 8px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: background-color .18s, transform .12s, color .12s;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .nav-links a:hover {
            transform: translateY(-2px);
            background: rgba(255,255,255,0.06);
        }

        .nav-links a.active {
            background: linear-gradient(90deg, rgba(255,255,255,0.12), rgba(255,255,255,0.06));
            box-shadow: 0 6px 18px rgba(11, 65, 132, 0.12);
            color: #fff;
        }

        /* make sure sections are not hidden under the sticky nav */
        section {
            scroll-margin-top: calc(var(--nav-height) + 12px);
        }
        
        /* Main Header (kept styling in case needed elsewhere) */
        .main-header {
            background: linear-gradient(135deg, var(--accent-1) 0%, var(--accent-2) 100%);
            color: white;
            padding: 2rem 3rem;
            text-align: center;
            box-shadow: 0 4px 20px rgba(0,0,0,0.15);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
        .main-header h1 {
            font-size: 2.5rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            text-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }
        
        /* Container */
        .container {
            max-width: 100%;
            width: 100%;
            margin: 0 auto;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--accent-1) 0%, var(--accent-2) 50%, var(--accent-3) 100%);
            color: white;
            padding: 6rem 3rem;
            text-align: center;
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
            background: radial-gradient(circle at 20% 50%, rgba(59, 130, 246, 0.18) 0%, transparent 40%),
                        radial-gradient(circle at 80% 80%, rgba(147, 197, 253, 0.12) 0%, transparent 50%);
            pointer-events: none;
        }
        
        .hero-content {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }
        
        .avatar {
            width: 180px;
            height: 180px;
            margin: 0 auto 2rem;
            background: linear-gradient(135deg, #ffffff 0%, #f1f5f9 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3), 0 0 0 8px rgba(255,255,255,0.1);
            border: 3px solid rgba(255,255,255,0.2);
        }
        
        .profile-photo {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            display: block;
        }
        
        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            text-shadow: 0 2px 20px rgba(0,0,0,0.2);
        }
        
        .hero .subtitle {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            opacity: 0.95;
            font-weight: 400;
        }
        
        .hero .location {
            font-size: 1.1rem;
            margin-bottom: 2rem;
            opacity: 0.85;
        }
        
        .cta-text {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            padding: 1.5rem 2.5rem;
            background: rgba(255,255,255,0.15);
            backdrop-filter: blur(10px);
            border-radius: 1rem;
            display: inline-block;
            border: 1px solid rgba(255,255,255,0.2);
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }
        
        .contact-links {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .contact-links a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: transform 0.3s;
            font-size: 1rem;
        }
        
        .contact-links a:hover {
            transform: translateY(-2px);
        }
        
        /* Section titles and layout */
        .section-title {
            font-size: 2.5rem;
            color: #0f172a;
            margin-bottom: 3rem;
            text-align: center;
            position: relative;
            padding-bottom: 1.5rem;
            font-weight: 700;
            letter-spacing: -0.02em;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 5px;
            background: linear-gradient(90deg, var(--accent-3) 0%, #60a5fa 100%);
            border-radius: 3px;
            box-shadow: 0 2px 10px rgba(59, 130, 246, 0.3);
        }

        /* small adjustments to ensure nav doesn't overlap content */
        @media (max-width: 768px) {
            :root { --nav-height: 56px; }
        }

        /* Rest of existing styles kept - education, skills, experience, achievements, projects, contact etc. */
        /* (omitted here for brevity in explanation, full styles below continue unchanged) */

        /* Education, Skills, Experience, Achievements, Projects, Contact styling (kept from previous) */
        .education-list { display:flex; flex-direction:column; gap:2rem; max-width:1400px; margin:0 auto; }
        .education-item { background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%); padding:2.5rem; border-radius:1rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); border-left:5px solid var(--accent-3); transition: all .4s; border:1px solid rgba(59,130,246,0.1); }
        .education-item:hover { transform: translateX(8px) translateY(-4px); box-shadow:0 12px 40px rgba(59,130,246,0.15); border-left-color:#2563eb; }
        .education-item h3 { margin-bottom:.5rem; }
        .education-item .institution { color:#6b7280; font-size:1.1rem; margin-bottom:.5rem; }
        .education-item .year { color:var(--accent-3); font-weight:600; }

        .skills-container { display:grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap:2rem; max-width:1400px; margin:0 auto; }
        .skill-category { background: linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); padding:2.5rem; border-radius:1.25rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); border:1px solid rgba(59,130,246,0.1); transition: all .4s; }
        .skill-category h3 { margin-bottom:1.5rem; display:flex; align-items:center; gap:.5rem; }
        .skill-list { display:flex; flex-wrap:wrap; gap:.75rem; }
        .skill-tag { background: linear-gradient(135deg,#dbeafe 0%, #bfdbfe 100%); color:#1e3a8a; padding:.65rem 1.25rem; border-radius:2rem; font-size:.9rem; font-weight:600; border:1px solid rgba(59,130,246,0.2); box-shadow:0 2px 8px rgba(59,130,246,0.1); }

        .experience-list { display:flex; flex-direction:column; gap:2rem; max-width:1400px; margin:0 auto; }
        .experience-item { background: linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); padding:2.5rem; border-radius:1.25rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); transition: all .4s; border:1px solid rgba(59,130,246,0.1); position:relative; overflow:hidden; }
        .experience-item::before { content:''; position:absolute; top:0; left:0; width:5px; height:100%; background: linear-gradient(180deg, var(--accent-3) 0%, #60a5fa 100%); transform: scaleY(0); transition: transform .4s ease; }
        .experience-item:hover { transform: translateY(-8px); box-shadow:0 12px 40px rgba(59,130,246,0.15); }
        .experience-item:hover::before { transform: scaleY(1); }
        .experience-header { display:flex; justify-content:space-between; align-items:start; margin-bottom:1rem; flex-wrap:wrap; gap:1rem; }
        .company { color:#6b7280; font-size:1.1rem; }
        .experience-type { background-color:#dbeafe; color:#1e3a8a; padding:.25rem .75rem; border-radius:1rem; font-size:.9rem; font-weight:600; }

        .achievements-grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap:1.5rem; max-width:1400px; margin:0 auto; }
        .achievement-card { background:linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); padding:2rem; border-radius:1.25rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); border-top:4px solid var(--accent-3); transition: all .4s; border:1px solid rgba(59,130,246,0.1); }
        .achievement-card:hover { transform: translateY(-8px); box-shadow:0 12px 40px rgba(59,130,246,0.2); border-top-color:#2563eb; }

        .extracurricular-list { display:grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap:1.5rem; max-width:1400px; margin:0 auto; }
        .extracurricular-item { background:linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); padding:2rem; border-radius:1rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); transition: all .4s; border:1px solid rgba(59,130,246,0.1); }

        .projects-grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap:2rem; max-width:1400px; margin:0 auto; }
        .project-card { background:linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); border-radius:1.5rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); overflow:hidden; transition: all .4s; border:1px solid rgba(59,130,246,0.1); }
        .project-header { background: linear-gradient(135deg, var(--accent-1) 0%, var(--accent-2) 50%, var(--accent-3) 100%); color:white; padding:2rem; position:relative; overflow:hidden; }
        .project-body { padding:1.5rem; }
        .view-details-btn { background-color: var(--accent-3); color:white; border:none; padding:.5rem 1.5rem; border-radius:.25rem; cursor:pointer; font-weight:600; width:100%; }

        .contact-container { max-width:1000px; margin:0 auto; }
        .contact-info { background: linear-gradient(135deg,#ffffff 0%, #f8fafc 100%); padding:2.5rem; border-radius:1.25rem; box-shadow:0 4px 20px rgba(0,0,0,0.08); border:1px solid rgba(59,130,246,0.1); }

        footer { background: linear-gradient(135deg,var(--accent-1) 0%, var(--accent-2) 100%); color:white; text-align:center; padding:3rem 1.5rem; border-top:1px solid rgba(255,255,255,0.1); box-shadow:0 -4px 20px rgba(0,0,0,0.1); }

        /* DESIGN gallery styles (kept / adjusted) */
        .gallery-header { background: linear-gradient(135deg,var(--accent-1) 0%, var(--accent-2) 100%); color:white; padding:1.25rem 1rem; text-align:center; box-shadow:0 4px 20px rgba(0,0,0,0.12); border-radius:10px; max-width:1200px; margin:0 auto 1.25rem; }
        .gallery-header h1 { font-size:1.9rem; font-weight:700; margin:0; letter-spacing:-0.02em; text-shadow:0 2px 8px rgba(0,0,0,0.15); }

        #design-gallery #info { text-align:center; margin-bottom:1.25rem; color:#334155; font-size:0.95rem; max-width:1200px; margin-left:auto; margin-right:auto; }
        #design-gallery #gallery { display:grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap:12px; max-width:1200px; margin:0 auto; }
        #design-gallery #gallery a { display:block; background:white; border-radius:8px; overflow:hidden; box-shadow:0 4px 10px rgba(2,6,23,0.06); transition: transform .18s, box-shadow .18s; text-decoration:none; }
        #design-gallery #gallery a:hover { transform: translateY(-6px); box-shadow:0 10px 22px rgba(2,6,23,0.12); }
        #design-gallery #gallery img { width:100%; height:160px; object-fit:cover; display:block; vertical-align:middle; }
        #design-gallery .filename { padding:8px 10px; font-size:0.87rem; color:#1f2937; white-space:nowrap; overflow:hidden; text-overflow:ellipsis; }
        #design-gallery #error { color:#b91c1c; text-align:center; margin-top:1rem; }
        @media (max-width:480px){ #design-gallery #gallery img{ height:120px } }

    </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
  <script src="https://cdn.tailwindcss.com" type="text/javascript"></script>
 </head>
 <body>
  <!-- Top navigation with anchor links (sticky) -->
  <nav class="top-nav" aria-label="Page sections">
    <div class="nav-inner">
      <div class="nav-links" role="navigation" aria-label="Primary">
        <a href="#about" data-target="about">About Me</a>
        <a href="#education" data-target="education">Education</a>
        <a href="#experience" data-target="experience">Experience</a>
        <a href="#achievements" data-target="achievements">Achievements &amp; Training</a>
        <a href="#extracurriculars" data-target="extracurriculars">Leadership &amp; Extracurriculars</a>
        <a href="#projects" data-target="projects">Projects</a>
        <a href="#contact" data-target="contact">Contact Me</a>
      </div>
    </div>
  </nav>

  <main class="container"><!-- Hero Section -->
   <section class="hero" id="top-hero">
    <div class="hero-content">
     <div class="avatar" role="img" aria-label="Profile picture of Md. Abdul Fahad"><img src="./phot%20for%20github/Md.%20Abdul%20Fahad.jpg" alt="Md. Abdul Fahad" class="profile-photo" onerror="this.style.display='none'; this.parentElement.innerHTML='<svg width=&#39;100&#39; height=&#39;100&#39; viewBox=&#39;0 0 100 100&#39; fill=&#39;none&#39; xmlns=&#39;http://www.w3.org/2000/svg&#39;><circle cx=&#39;50&#39; cy=&#39;35&#39; r=&#39;20&#39; fill=&#39;#1e3a8a&#39;/><path d=&#39;M20 85 C20 65, 30 55, 50 55 C70 55, 80 65, 80 85 Z&#39; fill=&#39;#1e3a8a&#39;/></svg>';">
     </div>
     <h2>Md. Abdul Fahad</h2>
     <p class="subtitle">Final-year BBA Student at BAUST</p>
     <p class="location">📍 Nilphamari, Saidpur, Rangpur, Bangladesh</p>
     <div class="cta-text">
      Seeking leadership internship opportunities — Let's connect.
     </div>
     <div class="contact-links">
       <a href="mailto:mdabdulfahad41@gmail.com" aria-label="Email Md. Abdul Fahad"> 📧 mdabdulfahad41@gmail.com </a>
       <a href="tel:+8801811435756" aria-label="Call Md. Abdul Fahad"> 📱 +৮ ৮ ০ ১ ৮ ১ ১ ৪ ৩ ৫ ৭ ৫ ৬ </a>
       <a href="https://www.linkedin.com/in/md-abdul-fahad" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn profile"> 💼 LinkedIn </a>
     </div>
    </div>
   </section>

   <section id="about" aria-labelledby="about-heading">
    <h2 id="about-heading" class="section-title">About Me</h2>
    <div class="about-content">
     <p>Enthusiastic final-year BBA student at Bangladesh Army University of Science &amp; Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.</p>
    </div>
   </section>

   <section id="education" aria-labelledby="education-heading">
    <h2 id="education-heading" class="section-title">Education</h2>
    <div class="education-list">
     <article class="education-item">
      <h3>Bachelor of Business Administration (BBA)</h3>
      <p class="institution">Bangladesh Army University of Science &amp; Technology (BAUST)</p>
      <p class="year">2022 – Present</p>
     </article>
     <article class="education-item">
      <h3>Higher Secondary Certificate (HSC)</h3>
      <p class="institution">Naogaon Government College</p>
      <p class="year">2021</p>
     </article>
     <article class="education-item">
      <h3>Secondary School Certificate (SSC)</h3>
      <p class="institution">Simanto Public School</p>
      <p class="year">2019</p>
     </article>
    </div>
   </section>

   <section id="skills" aria-labelledby="skills-heading">
    <h2 id="skills-heading" class="section-title">Skills</h2>
    <div class="skills-container">
     <article class="skill-category">
      <h3>💻 Technical Skills</h3>
      <div class="skill-list"><span class="skill-tag">Microsoft Word</span> <span class="skill-tag">Microsoft Excel</span> <span class="skill-tag">Microsoft PowerPoint</span> <span class="skill-tag">Canva</span> <span class="skill-tag">Google Workspace</span> <span class="skill-tag">Power BI (Basic)</span>
      </div>
     </article>
     <article class="skill-category">
      <h3>🤝 Soft Skills</h3>
      <div class="skill-list"><span class="skill-tag">Active Listening</span> <span class="skill-tag">Problem Solving</span> <span class="skill-tag">Time Management</span> <span class="skill-tag">Teamwork</span> <span class="skill-tag">Adaptability</span>
      </div>
     </article>
    </div>
   </section>

   <section id="experience" aria-labelledby="experience-heading">
    <h2 id="experience-heading" class="section-title">Experience</h2>
    <div class="experience-list">
     <article class="experience-item">
      <div class="experience-header">
       <div>
        <h3>Content Creator &amp; Designer</h3>
        <p class="company">Opportunity Point</p>
       </div><span class="experience-type">Remote</span>
      </div>
      <ul>
       <li>Managed e-book publishing projects from concept to completion</li>
       <li>Created engaging content for digital publications</li>
       <li>Designed professional graphics and layouts using Canva</li>
       <li>Collaborated with team members to ensure quality deliverables</li>
      </ul>
     </article>
     <article class="experience-item">
      <div class="experience-header">
       <div>
        <h3>Training Coordinator</h3>
        <p class="company">Bangladesh Youth Skills Development Organization (BYSDO)</p>
       </div><span class="experience-type">Remote</span>
      </div>
      <ul>
       <li>Conducted Google Forms training sessions for team members</li>
       <li>Implemented AI automation solutions to streamline workflows</li>
       <li>Managed task completion and quality assurance processes</li>
       <li>Provided technical support and guidance to participants</li>
      </ul>
     </article>
     <article class="experience-item">
      <div class="experience-header">
       <div>
        <h3>Operations Management</h3>
        <p class="company">YSSE</p>
       </div><span class="experience-type">Remote</span>
      </div>
      <ul>
       <li>Coordinated operational activities and team communications</li>
       <li>Managed project timelines and deliverables</li>
       <li>Supported organizational initiatives and events</li>
       <li>Contributed to process improvement and efficiency</li>
      </ul>
     </article>
    </div>
   </section>

   <section id="achievements" aria-labelledby="achievements-heading">
    <h2 id="achievements-heading" class="section-title">Achievements &amp; Training</h2>
    <div class="achievements-grid">
     <article class="achievement-card">
      <div class="achievement-icon">📊</div>
      <h3>BRAC ISD Excel Training</h3>
      <p>Completed advanced Excel training program focusing on data analysis and visualization techniques</p>
     </article>
     <article class="achievement-card">
      <div class="achievement-icon">💼</div>
      <h3>BRAC Career Hub Job Readiness Training</h3>
      <p>Enhanced professional skills including resume writing, interview preparation, and workplace communication</p>
     </article>
     <article class="achievement-card">
      <div class="achievement-icon">🎮</div>
      <h3>Revas Business Simulation</h3>
      <p>Participated in virtual business simulation (May 2025), managing strategic decisions for a travel agency</p>
     </article>
     <article class="achievement-card">
      <div class="achievement-icon">🤖</div>
      <h3>Agent X AI Competition</h3>
      <p>Competed in AI-focused competition (June 2025), demonstrating innovation and technical problem-solving</p>
     </article>
     <article class="achievement-card">
      <div class="achievement-icon">🏆</div>
      <h3>Business Case Competition</h3>
      <p>Organized and participated in business case competitions, showcasing analytical and presentation skills</p>
     </article>
     <article class="achievement-card">
      <div class="achievement-icon">⭐</div>
      <h3>Best Sub-Leader Award</h3>
      <p>Recognized as Best Sub-Leader in Campus Ambassador Program 2025 for outstanding leadership and performance</p>
     </article>
    </div>
   </section>

   <section id="extracurriculars" aria-labelledby="extracurriculars-heading">
    <h2 id="extracurriculars-heading" class="section-title">Leadership &amp; Extracurriculars</h2>
    <div class="extracurricular-list">
     <article class="extracurricular-item">
      <h3>🎯 General Secretary</h3>
      <p><strong>BAUST Business Club</strong></p>
      <p>Leading club activities, organizing events, and fostering business education among students</p>
     </article>
     <article class="extracurricular-item">
      <h3>👥 Executive Member</h3>
      <p><strong>Career Society of BAUST</strong></p>
      <p>Supporting career development initiatives and professional networking opportunities for students</p>
     </article>
     <article class="extracurricular-item">
      <h3>🎖️ BNCC Cadet</h3>
      <p><strong>Bangladesh National Cadet Corps</strong></p>
      <p>Developing leadership, discipline, and teamwork through military-style training and activities</p>
     </article>
     <article class="extracurricular-item">
      <h3>🎤 Seminar Organizer</h3>
      <p><strong>"Building a Future-Proof Career"</strong></p>
      <p>Successfully organized seminar with 300+ attendees, featuring industry experts and career guidance</p>
     </article>
     <article class="extracurricular-item">
      <h3>🤝 Job Fair Volunteer</h3>
      <p><strong>BAUST Career Fair</strong></p>
      <p>Assisted in coordinating job fair activities, connecting students with potential employers</p>
     </article>
    </div>
   </section>

   <section id="projects" aria-labelledby="projects-heading">
    <h2 id="projects-heading" class="section-title">Projects</h2>
    <div class="projects-grid">
     <article class="project-card" data-project="ebook">
      <div class="project-header">
       <h3>E-book Publishing Platform</h3>
       <p class="project-role">Content Creator &amp; Designer</p>
      </div>
      <div class="project-body">
       <p class="project-description">Managed end-to-end e-book publishing process including content creation, graphic design, and digital distribution for Opportunity Point.</p>
       <div class="project-outcome"><strong>Outcome:</strong> Successfully published multiple e-books with professional layouts and engaging content, reaching diverse audiences</div>
       <button class="view-details-btn" aria-label="View details for E-book Publishing Platform project">View Details</button>
      </div>
     </article>
     <article class="project-card" data-project="automation">
      <div class="project-header">
       <h3>Google Forms &amp; AI Automation</h3>
       <p class="project-role">Training Coordinator</p>
      </div>
      <div class="project-body">
       <p class="project-description">Developed and delivered training programs on Google Forms and AI automation tools for BYSDO team members, streamlining data collection and workflow processes.</p>
       <div class="project-outcome"><strong>Outcome:</strong> Improved team efficiency by 40% through automated workflows and reduced manual data entry tasks</div>
       <button class="view-details-btn" aria-label="View details for Google Forms &amp; AI Automation project">View Details</button>
      </div>
     </article>
     <article class="project-card" data-project="revas">
      <div class="project-header">
       <h3>Revas Business Simulation</h3>
       <p class="project-role">Strategic Decision Maker</p>
      </div>
      <div class="project-body">
       <p class="project-description">Participated in virtual travel agency simulation, making strategic decisions on pricing, marketing, operations, and resource allocation in a competitive market environment.</p>
       <div class="project-outcome"><strong>Outcome:</strong> Achieved top quartile performance through data-driven decision making and strategic planning</div>
       <button class="view-details-btn" aria-label="View details for Revas Business Simulation project">View Details</button>
      </div>
     </article>
    </div>
   </section>

   <!-- DESIGN Gallery Section -->
   <section id="design-gallery" aria-labelledby="design-gallery-heading">
     <div class="gallery-header">
       <h1 id="design-gallery-heading">DESIGN Gallery</h1>
     </div>
     <div id="info">Loading images from /DESIGN/ … (এটি পাবলিক রিপোর জন্য GitHub API ব্যবহার করে)</div>
     <div id="gallery" aria-live="polite"></div>
     <div id="error" role="alert"></div>
     <footer>If some images don't show, try a hard refresh (Ctrl/Cmd+Shift+R). Rate-limit: 60 unauth requests/hour.</footer>
   </section>

   <section id="contact" aria-labelledby="contact-heading">
    <h2 id="contact-heading" class="section-title">Contact Me</h2>
    <div class="contact-container">
     <div class="contact-info">
      <h3>Get In Touch</h3>
      <div class="contact-item"><span>📧</span> <a href="mailto:mdabdulfahad41@gmail.com">mdabdulfahad41@gmail.com</a></div>
      <div class="contact-item"><span>📱</span> <a href="tel:+8801811435756">+৮ ৮ ০ ১ ৮ ১ ১ ৪ ৩ ৫ ৭ ৫ ৬</a></div>
      <div class="contact-item"><span>💼</span> <a href="https://www.linkedin.com/in/md-abdul-fahad" target="_blank" rel="noopener noreferrer">linkedin.com/in/md-abdul-fahad</a></div>
      <div class="contact-item"><span>📍</span> <span>Nilphamari, Saidpur, Rangpur, Bangladesh</span></div>
     </div>
    </div>
   </section>

  </main>

  <footer>
   <p>© 2025 Md. Abdul Fahad. All rights reserved.</p>
   <p>Built with passion and dedication</p>
  </footer>

  <!-- Modal (project details) -->
  <div class="modal" id="projectModal" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
   <div class="modal-content">
    <div class="modal-header">
     <h3 id="modalTitle"></h3><button class="modal-close" aria-label="Close modal">×</button>
    </div>
    <div class="modal-body" id="modalBody"></div>
   </div>
  </div>

  <script>
    // small utility: highlight nav links on scroll using IntersectionObserver
    (function () {
      const navLinks = document.querySelectorAll('.nav-links a');
      const sections = Array.from(navLinks).map(a => document.getElementById(a.dataset.target));
      // fallback: if some targets don't exist, observe typical section IDs
      const observedSections = sections.filter(Boolean);

      const options = {
        root: null,
        rootMargin: '0px',
        threshold: 0.45 // section is considered active when ~45% visible
      };

      const observer = new IntersectionObserver((entries) => {
        // find entry with highest intersectionRatio that's intersecting
        const visible = entries.filter(e => e.isIntersecting);
        if (visible.length) {
          visible.sort((a,b) => b.intersectionRatio - a.intersectionRatio);
          const id = visible[0].target.id;
          navLinks.forEach(link => link.classList.toggle('active', link.dataset.target === id));
        }
      }, options);

      observedSections.forEach(s => observer.observe(s));

      // smooth scroll for older browsers & keep active class on click
      navLinks.forEach(link => {
        link.addEventListener('click', (e) => {
          // default smooth behavior is handled by CSS, but ensure focus & small offset if needed
          // do not prevent default so anchor hash updates; but set active immediately.
          navLinks.forEach(l => l.classList.remove('active'));
          link.classList.add('active');
        });
      });

      // on page load, set active based on current scroll/hash
      window.addEventListener('load', () => {
        const hash = location.hash.replace('#','');
        if (hash) {
          navLinks.forEach(l => l.classList.toggle('active', l.dataset.target === hash));
        } else {
          // if none, set About active by default
          navLinks.forEach(l => l.classList.toggle('active', l.dataset.target === 'about'));
        }
      });
    })();
  </script>

  <!-- existing scripts (project modal, elementSdk, design gallery loader) -->
  <script>
        // Configuration object
        const defaultConfig = {
            main_heading: "My Design",
            hero_headline: "Md. Abdul Fahad",
            hero_cta: "Seeking leadership internship opportunities — Let's connect.",
            career_objective: "Enthusiastic final-year BBA student at Bangladesh Army University of Science & Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.",
            email_address: "mdabdulfahad41@gmail.com",
            phone_number: "+৮ ৮ ০ ১ ৮ ১ ১ ৪ ৩ ৫ ৭ ৫ ৬",
            linkedin_url: "https://www.linkedin.com/in/md-abdul-fahad"
        };

        // helper: convert Bangla digits to ASCII digits
        function bnToEnDigits(str) {
            if (!str) return str;
            const map = {'০':'0','১':'1','২':'2','৩':'3','৪':'4','৫':'5','৬':'6','৭':'7','৮':'8','৯':'9'};
            return String(str).replace(/[০১২৩৪৫৬৭৮৯]/g, m => map[m]);
        }

        // Project modal functionality
        const modal = document.getElementById('projectModal');
        const modalTitle = document.getElementById('modalTitle');
        const modalBody = document.getElementById('modalBody');
        const modalClose = document.querySelector('.modal-close');

        const projectDetails = {
            ebook: {
                title: 'E-book Publishing Platform',
                content: `
                    <h4>Project Overview</h4>
                    <p>Led comprehensive e-book publishing initiatives for Opportunity Point, managing the complete lifecycle from content ideation to final distribution.</p>
                    <h4>Key Responsibilities</h4>
                    <ul>
                        <li>Developed engaging content across multiple genres and topics</li>
                        <li>Created professional layouts and cover designs using Canva</li>
                        <li>Managed quality assurance and editing processes</li>
                        <li>Coordinated with team members for timely project delivery</li>
                        <li>Implemented feedback loops to improve content quality</li>
                    </ul>
                `
            },
            automation: {
                title: 'Google Forms & AI Automation',
                content: '<p>Google Forms & AI Automation details...</p>'
            },
            revas: {
                title: 'Revas Business Simulation',
                content: '<p>Revas Business Simulation details...</p>'
            }
        };

        document.querySelectorAll('.view-details-btn').forEach(btn => {
            btn.addEventListener('click', (e) => {
                e.stopPropagation();
                const projectCard = btn.closest('.project-card');
                const projectId = projectCard.dataset.project;
                const project = projectDetails[projectId];
                
                if (project) {
                    modalTitle.textContent = project.title;
                    modalBody.innerHTML = project.content;
                    modal.classList.add('active');
                    document.body.style.overflow = 'hidden';
                }
            });
        });

        modalClose.addEventListener('click', () => {
            modal.classList.remove('active');
            document.body.style.overflow = '';
        });

        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                modal.classList.remove('active');
                document.body.style.overflow = '';
            }
        });

        // Element SDK onConfigChange (updates contact info, hero text, etc.)
        async function onConfigChange(config) {
            const heroHeadline = document.querySelector('.hero h2');
            const ctaText = document.querySelector('.cta-text');
            const careerObjective = document.querySelector('.about-content p');
            const emailLinks = document.querySelectorAll('a[href^="mailto:"]');
            const phoneLinks = document.querySelectorAll('a[href^="tel:"]');
            const linkedinLinks = document.querySelectorAll('a[href*="linkedin.com"]');
            const emailDisplays = document.querySelectorAll('.contact-links a[href^="mailto:"], .contact-item a[href^="mailto:"]');
            const phoneDisplays = document.querySelectorAll('.contact-links a[href^="tel:"], .contact-item a[href^="tel:"]');

            if (heroHeadline) {
                heroHeadline.textContent = config.hero_headline || defaultConfig.hero_headline;
            }

            if (ctaText) {
                ctaText.textContent = config.hero_cta || defaultConfig.hero_cta;
            }

            if (careerObjective) {
                careerObjective.textContent = config.career_objective || defaultConfig.career_objective;
            }

            const email = config.email_address || defaultConfig.email_address;
            emailLinks.forEach(link => link.href = `mailto:${email}`);
            emailDisplays.forEach(display => display.textContent = email);

            const phoneRaw = config.phone_number || defaultConfig.phone_number;
            const phoneAscii = bnToEnDigits(phoneRaw);
            const phoneHref = (phoneAscii || '').replace(/\s+/g, '').replace(/[^+\d]/g, '');
            phoneLinks.forEach(link => link.href = `tel:${phoneHref}`);
            phoneDisplays.forEach(display => display.textContent = phoneRaw);

            const linkedin = config.linkedin_url || defaultConfig.linkedin_url;
            linkedinLinks.forEach(link => link.href = linkedin);
        }

        if (window.elementSdk) {
            window.elementSdk.init({
                defaultConfig: defaultConfig,
                onConfigChange: onConfigChange,
                mapToCapabilities: (config) => ({ recolorables: [], borderables: [], fontEditable: undefined, fontSizeable: undefined }),
                mapToEditPanelValues: (config) => new Map([
                    ["main_heading", config.main_heading || defaultConfig.main_heading],
                    ["hero_headline", config.hero_headline || defaultConfig.hero_headline],
                    ["hero_cta", config.hero_cta || defaultConfig.hero_cta],
                    ["career_objective", config.career_objective || defaultConfig.career_objective],
                    ["email_address", config.email_address || defaultConfig.email_address],
                    ["phone_number", config.phone_number || defaultConfig.phone_number],
                    ["linkedin_url", config.linkedin_url || defaultConfig.linkedin_url]
                ])
            });
        }

    </script>

  <!-- DESIGN gallery loader (unchanged) -->
  <script>
    (async function(){
      const owner = "fahad220211041";
      const repo = "fahad220211041.github.io";
      const path = "DESIGN";
      const apiUrl = `https://api.github.com/repos/${owner}/${repo}/contents/${encodeURIComponent(path)}`;

      const infoEl = document.querySelector("#design-gallery #info");
      const gallery = document.querySelector("#design-gallery #gallery");
      const errorEl = document.querySelector("#design-gallery #error");

      try {
        const res = await fetch(apiUrl);
        if (!res.ok) {
          throw new Error("GitHub API error: " + res.status + " " + res.statusText);
        }
        const files = await res.json();

        const imageExt = [".png", ".jpg", ".jpeg", ".gif", ".webp", ".svg"];
        const images = Array.isArray(files) ? files.filter(f => {
          const n = f.name.toLowerCase();
          return imageExt.some(ext => n.endsWith(ext));
        }) : [];

        if (images.length === 0) {
          infoEl.textContent = "এই ফোল্ডারে কোনো ছবি পাওয়া যায়নি (বা নাম/পাথ ভুল)।";
          return;
        }

        infoEl.textContent = `Found ${images.length} image(s) in /${path}/ — click to open full size.`;

        images.sort((a,b) => a.name.localeCompare(b.name, undefined, {numeric:true, sensitivity:'base'}));

        images.forEach(file => {
          const link = document.createElement("a");
          link.href = file.download_url;
          link.target = "_blank";
          link.rel = "noopener noreferrer";

          const img = document.createElement("img");
          img.src = file.download_url;
          img.alt = file.name;
          img.loading = "lazy";

          const caption = document.createElement("div");
          caption.className = "filename";
          caption.textContent = file.name;

          link.appendChild(img);
          link.appendChild(caption);
          gallery.appendChild(link);
        });

      } catch (err) {
        console.error(err);
        if (infoEl) infoEl.textContent = "";
        if (errorEl) {
          errorEl.textContent = "চিত্রগুলো লোড করতে সমস্যা হয়েছে: " + err.message;
          errorEl.innerHTML += "<br/>(Note: GitHub API rate limits unauthenticated requests to ~60/hour.)";
        }
      }
    })();
  </script>

 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'99b518e081bedaf6',t:'MTc2MjYwNTE4OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
