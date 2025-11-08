<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Portfolio</title>
  <script src="/_sdk/element_sdk.js"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
        body {
            box-sizing: border-box;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .skill-bar {
            height: 8px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 4px;
            transition: width 0.8s ease;
        }
        
        .section-fade {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }
        
        .section-fade.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="min-h-full bg-gray-50"><!-- Navigation -->
  <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
   <div class="max-w-6xl mx-auto px-4">
    <div class="flex justify-between items-center py-4">
     <div class="text-xl font-bold text-gray-800" id="nav-name">
      Alex Johnson
     </div>
     <div class="hidden md:flex space-x-8"><a href="#about" class="text-gray-600 hover:text-blue-600 transition-colors">About</a> <a href="#projects" class="text-gray-600 hover:text-blue-600 transition-colors">Projects</a> <a href="#skills" class="text-gray-600 hover:text-blue-600 transition-colors">Skills</a> <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors">Contact</a>
     </div><button id="mobile-menu-btn" class="md:hidden text-gray-600">
      <svg class="w-6 h-6" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
      </svg></button>
    </div>
    <div id="mobile-menu" class="md:hidden hidden pb-4"><a href="#about" class="block py-2 text-gray-600 hover:text-blue-600">About</a> <a href="#projects" class="block py-2 text-gray-600 hover:text-blue-600">Projects</a> <a href="#skills" class="block py-2 text-gray-600 hover:text-blue-600">Skills</a> <a href="#contact" class="block py-2 text-gray-600 hover:text-blue-600">Contact</a>
    </div>
   </div>
  </nav><!-- Hero Section -->
  <section class="gradient-bg text-white pt-24 pb-20">
   <div class="max-w-6xl mx-auto px-4 text-center">
    <div class="mb-8">
     <div class="w-32 h-32 bg-white rounded-full mx-auto mb-6 flex items-center justify-center text-6xl">
      👨‍🎓
     </div>
     <h1 class="text-5xl font-bold mb-4" id="hero-name">Alex Johnson</h1>
     <p class="text-xl mb-8" id="hero-tagline">Computer Science Student &amp; Web Developer</p>
     <div class="flex justify-center space-x-4"><a href="#contact" class="bg-white text-blue-600 px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition-colors"> Get In Touch </a> <a href="#projects" class="border-2 border-white text-white px-8 py-3 rounded-lg font-semibold hover:bg-white hover:text-blue-600 transition-colors"> View Projects </a>
     </div>
    </div>
   </div>
  </section><!-- About Section -->
  <section id="about" class="py-20 bg-white">
   <div class="max-w-6xl mx-auto px-4">
    <div class="section-fade">
     <h2 class="text-4xl font-bold text-center mb-16 text-gray-800">About Me</h2>
     <div class="grid md:grid-cols-2 gap-12 items-center">
      <div>
       <p class="text-lg text-gray-600 mb-6" id="about-description">I'm a passionate Computer Science student with a love for creating innovative web solutions. Currently pursuing my degree while building real-world projects that solve meaningful problems. I enjoy learning new technologies and collaborating with others to bring ideas to life.</p>
       <div class="grid grid-cols-2 gap-4 text-center">
        <div class="bg-gray-50 p-4 rounded-lg">
         <div class="text-2xl font-bold text-blue-600">
          3.8
         </div>
         <div class="text-gray-600">
          GPA
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg">
         <div class="text-2xl font-bold text-blue-600">
          15+
         </div>
         <div class="text-gray-600">
          Projects
         </div>
        </div>
       </div>
      </div>
      <div class="text-center">
       <div class="text-8xl mb-4">
        🚀
       </div>
       <h3 class="text-2xl font-semibold mb-4 text-gray-800">Always Learning</h3>
       <p class="text-gray-600">Constantly exploring new technologies and pushing the boundaries of what's possible.</p>
      </div>
     </div>
    </div>
   </div>
  </section><!-- Projects Section -->
  <section id="projects" class="py-20 bg-gray-50">
   <div class="max-w-6xl mx-auto px-4">
    <div class="section-fade">
     <h2 class="text-4xl font-bold text-center mb-16 text-gray-800">Featured Projects</h2>
     <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8"><!-- Project 1 -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
       <div class="h-48 bg-gradient-to-br from-blue-400 to-purple-500 flex items-center justify-center text-6xl">
        🌐
       </div>
       <div class="p-6">
        <h3 class="text-xl font-semibold mb-2">E-Commerce Platform</h3>
        <p class="text-gray-600 mb-4">Full-stack web application with React, Node.js, and MongoDB. Features user authentication, payment processing, and admin dashboard.</p>
        <div class="flex flex-wrap gap-2 mb-4"><span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-sm">React</span> <span class="bg-green-100 text-green-800 px-2 py-1 rounded text-sm">Node.js</span> <span class="bg-yellow-100 text-yellow-800 px-2 py-1 rounded text-sm">MongoDB</span>
        </div>
        <div class="flex space-x-3"><button class="text-blue-600 hover:text-blue-800 font-medium">Live Demo</button> <button class="text-gray-600 hover:text-gray-800 font-medium">GitHub</button>
        </div>
       </div>
      </div><!-- Project 2 -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
       <div class="h-48 bg-gradient-to-br from-green-400 to-blue-500 flex items-center justify-center text-6xl">
        📱
       </div>
       <div class="p-6">
        <h3 class="text-xl font-semibold mb-2">Task Management App</h3>
        <p class="text-gray-600 mb-4">Mobile-first progressive web app for team collaboration. Built with Vue.js and Firebase for real-time updates.</p>
        <div class="flex flex-wrap gap-2 mb-4"><span class="bg-green-100 text-green-800 px-2 py-1 rounded text-sm">Vue.js</span> <span class="bg-orange-100 text-orange-800 px-2 py-1 rounded text-sm">Firebase</span> <span class="bg-purple-100 text-purple-800 px-2 py-1 rounded text-sm">PWA</span>
        </div>
        <div class="flex space-x-3"><button class="text-blue-600 hover:text-blue-800 font-medium">Live Demo</button> <button class="text-gray-600 hover:text-gray-800 font-medium">GitHub</button>
        </div>
       </div>
      </div><!-- Project 3 -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
       <div class="h-48 bg-gradient-to-br from-purple-400 to-pink-500 flex items-center justify-center text-6xl">
        🤖
       </div>
       <div class="p-6">
        <h3 class="text-xl font-semibold mb-2">AI Study Assistant</h3>
        <p class="text-gray-600 mb-4">Machine learning application that helps students organize notes and generate study materials using natural language processing.</p>
        <div class="flex flex-wrap gap-2 mb-4"><span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-sm">Python</span> <span class="bg-red-100 text-red-800 px-2 py-1 rounded text-sm">TensorFlow</span> <span class="bg-gray-100 text-gray-800 px-2 py-1 rounded text-sm">NLP</span>
        </div>
        <div class="flex space-x-3"><button class="text-blue-600 hover:text-blue-800 font-medium">Live Demo</button> <button class="text-gray-600 hover:text-gray-800 font-medium">GitHub</button>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </section><!-- Skills Section -->
  <section id="skills" class="py-20 bg-white">
   <div class="max-w-6xl mx-auto px-4">
    <div class="section-fade">
     <h2 class="text-4xl font-bold text-center mb-16 text-gray-800">Skills &amp; Technologies</h2>
     <div class="grid md:grid-cols-2 gap-12">
      <div>
       <h3 class="text-2xl font-semibold mb-6 text-gray-800">Programming Languages</h3>
       <div class="space-y-4">
        <div>
         <div class="flex justify-between mb-2"><span class="text-gray-700">JavaScript</span> <span class="text-gray-500">90%</span>
         </div>
         <div class="bg-gray-200 rounded-full h-2">
          <div class="skill-bar w-[90%]"></div>
         </div>
        </div>
        <div>
         <div class="flex justify-between mb-2"><span class="text-gray-700">Python</span> <span class="text-gray-500">85%</span>
         </div>
         <div class="bg-gray-200 rounded-full h-2">
          <div class="skill-bar w-[85%]"></div>
         </div>
        </div>
        <div>
         <div class="flex justify-between mb-2"><span class="text-gray-700">Java</span> <span class="text-gray-500">80%</span>
         </div>
         <div class="bg-gray-200 rounded-full h-2">
          <div class="skill-bar w-[80%]"></div>
         </div>
        </div>
        <div>
         <div class="flex justify-between mb-2"><span class="text-gray-700">C++</span> <span class="text-gray-500">75%</span>
         </div>
         <div class="bg-gray-200 rounded-full h-2">
          <div class="skill-bar w-[75%]"></div>
         </div>
        </div>
       </div>
      </div>
      <div>
       <h3 class="text-2xl font-semibold mb-6 text-gray-800">Frameworks &amp; Tools</h3>
       <div class="grid grid-cols-2 gap-4">
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          ⚛️
         </div>
         <div class="font-medium">
          React
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          🟢
         </div>
         <div class="font-medium">
          Node.js
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          🐍
         </div>
         <div class="font-medium">
          Django
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          🍃
         </div>
         <div class="font-medium">
          MongoDB
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          🐙
         </div>
         <div class="font-medium">
          Git
         </div>
        </div>
        <div class="bg-gray-50 p-4 rounded-lg text-center">
         <div class="text-3xl mb-2">
          ☁️
         </div>
         <div class="font-medium">
          AWS
         </div>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </section><!-- Contact Section -->
  <section id="contact" class="py-20 bg-gray-50">
   <div class="max-w-4xl mx-auto px-4">
    <div class="section-fade">
     <h2 class="text-4xl font-bold text-center mb-16 text-gray-800">Get In Touch</h2>
     <div class="grid md:grid-cols-2 gap-12">
      <div>
       <h3 class="text-2xl font-semibold mb-6 text-gray-800">Let's Connect</h3>
       <p class="text-gray-600 mb-8">I'm always interested in new opportunities, collaborations, and interesting projects. Feel free to reach out if you'd like to work together or just want to say hello!</p>
       <div class="space-y-4">
        <div class="flex items-center space-x-3">
         <div class="text-2xl">
          📧
         </div><span class="text-gray-700" id="contact-email">alex.johnson@email.com</span>
        </div>
        <div class="flex items-center space-x-3">
         <div class="text-2xl">
          📱
         </div><span class="text-gray-700" id="contact-phone">+1 (555) 123-4567</span>
        </div>
        <div class="flex items-center space-x-3">
         <div class="text-2xl">
          💼
         </div><a href="#" class="text-blue-600 hover:text-blue-800" id="contact-linkedin">LinkedIn Profile</a>
        </div>
        <div class="flex items-center space-x-3">
         <div class="text-2xl">
          🐙
         </div><a href="#" class="text-blue-600 hover:text-blue-800" id="contact-github">GitHub Profile</a>
        </div>
       </div>
      </div>
      <div class="bg-white p-8 rounded-lg shadow-lg">
       <form id="contact-form">
        <div class="mb-6"><label for="name" class="block text-gray-700 font-medium mb-2">Name</label> <input type="text" id="name" name="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" required>
        </div>
        <div class="mb-6"><label for="email" class="block text-gray-700 font-medium mb-2">Email</label> <input type="email" id="email" name="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" required>
        </div>
        <div class="mb-6"><label for="message" class="block text-gray-700 font-medium mb-2">Message</label> <textarea id="message" name="message" rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" required></textarea>
        </div><button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors"> Send Message </button>
       </form>
       <div id="form-message" class="mt-4 text-center hidden"></div>
      </div>
     </div>
    </div>
   </div>
  </section><!-- Footer -->
  <footer class="bg-gray-800 text-white py-8">
   <div class="max-w-6xl mx-auto px-4 text-center">
    <p>© 2024 <span id="footer-name">Alex Johnson</span>. All rights reserved.</p>
    <p class="text-gray-400 mt-2">Built with passion and lots of coffee ☕</p>
   </div>
  </footer>
  <script>
        // Default configuration
        const defaultConfig = {
            student_name: "Alex Johnson",
            tagline: "Computer Science Student & Web Developer",
            about_text: "I'm a passionate Computer Science student with a love for creating innovative web solutions. Currently pursuing my degree while building real-world projects that solve meaningful problems. I enjoy learning new technologies and collaborating with others to bring ideas to life.",
            email_address: "alex.johnson@email.com",
            phone_number: "+1 (555) 123-4567",
            linkedin_url: "https://linkedin.com/in/alexjohnson",
            github_url: "https://github.com/alexjohnson"
        };

        // Mobile menu functionality
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
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
                    // Close mobile menu if open
                    mobileMenu.classList.add('hidden');
                }
            });
        });

        // Intersection Observer for fade-in animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.section-fade').forEach(el => {
            observer.observe(el);
        });

        // Contact form handling
        const contactForm = document.getElementById('contact-form');
        const formMessage = document.getElementById('form-message');

        contactForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Show success message
            formMessage.textContent = 'Thank you for your message! I\'ll get back to you soon.';
            formMessage.className = 'mt-4 text-center text-green-600 font-medium';
            formMessage.classList.remove('hidden');
            
            // Reset form
            contactForm.reset();
            
            // Hide message after 5 seconds
            setTimeout(() => {
                formMessage.classList.add('hidden');
            }, 5000);
        });

        // Update content based on config
        async function onConfigChange(config) {
            const name = config.student_name || defaultConfig.student_name;
            const tagline = config.tagline || defaultConfig.tagline;
            const aboutText = config.about_text || defaultConfig.about_text;
            const email = config.email_address || defaultConfig.email_address;
            const phone = config.phone_number || defaultConfig.phone_number;
            const linkedin = config.linkedin_url || defaultConfig.linkedin_url;
            const github = config.github_url || defaultConfig.github_url;

            // Update all name instances
            document.getElementById('nav-name').textContent = name;
            document.getElementById('hero-name').textContent = name;
            document.getElementById('footer-name').textContent = name;

            // Update tagline
            document.getElementById('hero-tagline').textContent = tagline;

            // Update about text
            document.getElementById('about-description').textContent = aboutText;

            // Update contact information
            document.getElementById('contact-email').textContent = email;
            document.getElementById('contact-phone').textContent = phone;
            
            const linkedinLink = document.getElementById('contact-linkedin');
            linkedinLink.textContent = 'LinkedIn Profile';
            linkedinLink.href = linkedin;
            
            const githubLink = document.getElementById('contact-github');
            githubLink.textContent = 'GitHub Profile';
            githubLink.href = github;
        }

        // Initialize Element SDK
        if (window.elementSdk) {
            window.elementSdk.init({
                defaultConfig: defaultConfig,
                onConfigChange: onConfigChange,
                mapToCapabilities: (config) => ({
                    recolorables: [],
                    borderables: [],
                    fontEditable: undefined,
                    fontSizeable: undefined
                }),
                mapToEditPanelValues: (config) => new Map([
                    ["student_name", config.student_name || defaultConfig.student_name],
                    ["tagline", config.tagline || defaultConfig.tagline],
                    ["about_text", config.about_text || defaultConfig.about_text],
                    ["email_address", config.email_address || defaultConfig.email_address],
                    ["phone_number", config.phone_number || defaultConfig.phone_number],
                    ["linkedin_url", config.linkedin_url || defaultConfig.linkedin_url],
                    ["github_url", config.github_url || defaultConfig.github_url]
                ])
            });
        }

        // Initial render
        onConfigChange(defaultConfig);
    </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9961eba8176033d3',t:'MTc2MTczMzAxOS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
