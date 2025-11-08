<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Md. Abdul Fahad - Final-year BBA student at BAUST seeking leadership internship opportunities. Experienced in business clubs, BNCC, and volunteering.">
  <meta property="og:title" content="Md. Abdul Fahad - Portfolio">
  <meta property="og:description" content="Final-year BBA student seeking leadership internship opportunities">
  <meta property="og:type" content="website">
  <title>Md. Abdul Fahad - Portfolio</title>
  <script src="/_sdk/element_sdk.js"></script>
  <style>
        /* README: HOW TO UPDATE THIS PORTFOLIO
         * 
         * 1. UPDATING CONTENT:
         *    - Find the section you want to edit (e.g., id="about", id="education")
         *    - Update text directly in the HTML
         *    - For contact info, update the links and text in the Contact section
         * 
         * 2. REPLACING PROFILE PHOTO:
         *    - Replace the SVG avatar in the hero section with an <img> tag
         *    - Example: <img src="your-photo.jpg" alt="Md. Abdul Fahad" class="profile-photo">
         *    - Add this CSS: .profile-photo { width: 200px; height: 200px; border-radius: 50%; object-fit: cover; }
         * 
         * 3. UPDATING CV DOWNLOAD LINK:
         *    - Find the "Download CV" button
         *    - Replace href="#" with href="your-cv.pdf"
         *    - Upload your CV PDF to the same folder as this HTML file
         * 
         * 4. CHANGING COLORS:
         *    - Primary color (navy): Search for #1e3a8a and replace
         *    - Accent color (blue): Search for #3b82f6 and replace
         *    - Background: Search for #f8fafc and replace
         * 
         * 5. HOSTING ON GITHUB PAGES:
         *    - Create a GitHub repository
         *    - Upload this file as index.html
         *    - Go to Settings > Pages > Select main branch
         *    - Your site will be live at username.github.io/repository-name
         */
        
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
        }
        
        /* Navigation */
        nav {
            background: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            color: white;
            padding: 1.25rem 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(0,0,0,0.15);
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }
        
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .nav-brand {
            font-size: 1.5rem;
            font-weight: bold;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
            align-items: center;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
            font-weight: 500;
        }
        
        .nav-links a:hover {
            color: #93c5fd;
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        .download-cv-btn {
            background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%);
            color: white;
            padding: 0.75rem 2rem;
            border-radius: 0.75rem;
            text-decoration: none;
            transition: all 0.3s ease;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(59, 130, 246, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .download-cv-btn:hover {
            background: linear-gradient(135deg, #2563eb 0%, #1d4ed8 100%);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(59, 130, 246, 0.4);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #3b82f6 100%);
            color: white;
            padding: 8rem 1.5rem 6rem;
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
            background: radial-gradient(circle at 20% 50%, rgba(59, 130, 246, 0.3) 0%, transparent 50%),
                        radial-gradient(circle at 80% 80%, rgba(147, 197, 253, 0.2) 0%, transparent 50%);
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
            margin: 0 auto 2.5rem;
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
            margin: 0;
            box-shadow: none;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            animation: fadeInUp 0.8s ease-out;
            text-shadow: 0 2px 20px rgba(0,0,0,0.2);
        }
        
        .hero .subtitle {
            font-size: 1.6rem;
            margin-bottom: 1rem;
            opacity: 0.95;
            font-weight: 400;
            animation: fadeInUp 0.8s ease-out 0.2s both;
        }
        
        .hero .location {
            font-size: 1.15rem;
            margin-bottom: 2.5rem;
            opacity: 0.85;
            animation: fadeInUp 0.8s ease-out 0.4s both;
        }
        
        .cta-text {
            font-size: 1.3rem;
            margin-bottom: 2.5rem;
            padding: 1.5rem 2.5rem;
            background: rgba(255,255,255,0.15);
            backdrop-filter: blur(10px);
            border-radius: 1rem;
            display: inline-block;
            animation: fadeInUp 0.8s ease-out 0.6s both;
            border: 1px solid rgba(255,255,255,0.2);
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }
        
        .contact-links {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
            animation: fadeInUp 0.8s ease-out 0.8s both;
        }
        
        .contact-links a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: transform 0.3s;
        }
        
        .contact-links a:hover {
            transform: translateY(-2px);
        }
        
        /* Sections */
        section {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 1.5rem;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.6s ease-out forwards;
        }
        
        section:nth-child(even) {
            background-color: white;
        }
        
        h2 {
            font-size: 2.75rem;
            color: #0f172a;
            margin-bottom: 3rem;
            text-align: center;
            position: relative;
            padding-bottom: 1.5rem;
            font-weight: 700;
            letter-spacing: -0.02em;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 5px;
            background: linear-gradient(90deg, #3b82f6 0%, #60a5fa 100%);
            border-radius: 3px;
            box-shadow: 0 2px 10px rgba(59, 130, 246, 0.3);
        }
        
        h3 {
            font-size: 1.5rem;
            color: #1e3a8a;
            margin-bottom: 1rem;
        }
        
        /* About Section */
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.1rem;
            line-height: 1.8;
            text-align: center;
        }
        
        /* Education Section */
        .education-list {
            display: flex;
            flex-direction: column;
            gap: 2rem;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .education-item {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2.5rem;
            border-radius: 1rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            border-left: 5px solid #3b82f6;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid rgba(59, 130, 246, 0.1);
        }
        
        .education-item:hover {
            transform: translateX(8px) translateY(-4px);
            box-shadow: 0 12px 40px rgba(59, 130, 246, 0.15);
            border-left-color: #2563eb;
        }
        
        .education-item h3 {
            margin-bottom: 0.5rem;
        }
        
        .education-item .institution {
            color: #6b7280;
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
        }
        
        .education-item .year {
            color: #3b82f6;
            font-weight: 600;
        }
        
        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .skill-category {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2.5rem;
            border-radius: 1.25rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            border: 1px solid rgba(59, 130, 246, 0.1);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .skill-category:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 40px rgba(59, 130, 246, 0.15);
        }
        
        .skill-category h3 {
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
        }
        
        .skill-tag {
            background: linear-gradient(135deg, #dbeafe 0%, #bfdbfe 100%);
            color: #1e3a8a;
            padding: 0.65rem 1.25rem;
            border-radius: 2rem;
            font-size: 0.9rem;
            font-weight: 600;
            border: 1px solid rgba(59, 130, 246, 0.2);
            transition: all 0.3s ease;
            box-shadow: 0 2px 8px rgba(59, 130, 246, 0.1);
        }
        
        .skill-tag:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(59, 130, 246, 0.2);
            background: linear-gradient(135deg, #bfdbfe 0%, #93c5fd 100%);
        }
        
        /* Experience Section */
        .experience-list {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }
        
        .experience-item {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2.5rem;
            border-radius: 1.25rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid rgba(59, 130, 246, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .experience-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: linear-gradient(180deg, #3b82f6 0%, #60a5fa 100%);
            transform: scaleY(0);
            transition: transform 0.4s ease;
        }
        
        .experience-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 40px rgba(59, 130, 246, 0.15);
        }
        
        .experience-item:hover::before {
            transform: scaleY(1);
        }
        
        .experience-header {
            display: flex;
            justify-content: space-between;
            align-items: start;
            margin-bottom: 1rem;
            flex-wrap: wrap;
            gap: 1rem;
        }
        
        .experience-item h3 {
            margin-bottom: 0.25rem;
        }
        
        .company {
            color: #6b7280;
            font-size: 1.1rem;
        }
        
        .experience-type {
            background-color: #dbeafe;
            color: #1e3a8a;
            padding: 0.25rem 0.75rem;
            border-radius: 1rem;
            font-size: 0.9rem;
            font-weight: 600;
        }
        
        .experience-item ul {
            margin-left: 1.5rem;
            margin-top: 1rem;
        }
        
        .experience-item li {
            margin-bottom: 0.5rem;
        }
        
        /* Achievements Section */
        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }
        
        .achievement-card {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2rem;
            border-radius: 1.25rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            border-top: 4px solid #3b82f6;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid rgba(59, 130, 246, 0.1);
            border-top: 4px solid #3b82f6;
        }
        
        .achievement-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 40px rgba(59, 130, 246, 0.2);
            border-top-color: #2563eb;
        }
        
        .achievement-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
        }
        
        .achievement-card h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }
        
        /* Extracurriculars Section */
        .extracurricular-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }
        
        .extracurricular-item {
            background-color: white;
            padding: 1.5rem;
            border-radius: 0.5rem;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .extracurricular-item:hover {
            transform: scale(1.02);
            box-shadow: 0 6px 12px rgba(0,0,0,0.15);
        }
        
        .extracurricular-item h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }
        
        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            border-radius: 1.5rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            border: 1px solid rgba(59, 130, 246, 0.1);
        }
        
        .project-card:hover {
            transform: translateY(-12px);
            box-shadow: 0 20px 60px rgba(59, 130, 246, 0.2);
        }
        
        .project-header {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #3b82f6 100%);
            color: white;
            padding: 2rem;
            position: relative;
            overflow: hidden;
        }
        
        .project-header::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            pointer-events: none;
        }
        
        .project-header h3 {
            color: white;
            margin-bottom: 0.5rem;
        }
        
        .project-role {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        .project-body {
            padding: 1.5rem;
        }
        
        .project-description {
            margin-bottom: 1rem;
            color: #4b5563;
        }
        
        .project-outcome {
            background-color: #f0fdf4;
            border-left: 3px solid #22c55e;
            padding: 0.75rem;
            margin-bottom: 1rem;
            border-radius: 0.25rem;
        }
        
        .project-outcome strong {
            color: #15803d;
        }
        
        .view-details-btn {
            background-color: #3b82f6;
            color: white;
            border: none;
            padding: 0.5rem 1.5rem;
            border-radius: 0.25rem;
            cursor: pointer;
            font-weight: 600;
            transition: background-color 0.3s;
            width: 100%;
        }
        
        .view-details-btn:hover {
            background-color: #2563eb;
        }
        
        /* Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.7);
            z-index: 2000;
            align-items: center;
            justify-content: center;
            padding: 1rem;
        }
        
        .modal.active {
            display: flex;
        }
        
        .modal-content {
            background-color: white;
            border-radius: 0.5rem;
            max-width: 600px;
            width: 100%;
            max-height: 90%;
            overflow-y: auto;
            position: relative;
            animation: modalSlideIn 0.3s ease-out;
        }
        
        .modal-header {
            background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);
            color: white;
            padding: 2rem;
            position: relative;
        }
        
        .modal-close {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: none;
            border: none;
            color: white;
            font-size: 2rem;
            cursor: pointer;
            line-height: 1;
            padding: 0;
            width: 2rem;
            height: 2rem;
        }
        
        .modal-body {
            padding: 2rem;
        }
        
        .modal-body h4 {
            color: #1e3a8a;
            margin-top: 1.5rem;
            margin-bottom: 0.75rem;
        }
        
        .modal-body ul {
            margin-left: 1.5rem;
        }
        
        .modal-body li {
            margin-bottom: 0.5rem;
        }
        
        /* Contact Section */
        .contact-container {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .contact-info {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2.5rem;
            border-radius: 1.25rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            border: 1px solid rgba(59, 130, 246, 0.1);
        }
        
        .contact-info h3 {
            margin-bottom: 1.5rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
            padding: 1rem 1.25rem;
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
            border-radius: 0.75rem;
            transition: all 0.3s ease;
            border: 1px solid rgba(59, 130, 246, 0.1);
        }
        
        .contact-item:hover {
            transform: translateX(5px);
            background: linear-gradient(135deg, #dbeafe 0%, #bfdbfe 100%);
            box-shadow: 0 4px 12px rgba(59, 130, 246, 0.15);
        }
        
        .contact-item a {
            color: #3b82f6;
            text-decoration: none;
            word-break: break-all;
        }
        
        .contact-item a:hover {
            text-decoration: underline;
        }
        
        .contact-form {
            background-color: white;
            padding: 2rem;
            border-radius: 0.5rem;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        
        .contact-form h3 {
            margin-bottom: 1.5rem;
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #374151;
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid #e5e7eb;
            border-radius: 0.25rem;
            font-family: inherit;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        
        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #3b82f6;
        }
        
        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }
        
        .error-message {
            color: #dc2626;
            font-size: 0.875rem;
            margin-top: 0.25rem;
            display: none;
        }
        
        .form-group.error input,
        .form-group.error textarea {
            border-color: #dc2626;
        }
        
        .form-group.error .error-message {
            display: block;
        }
        
        .submit-btn {
            background-color: #3b82f6;
            color: white;
            border: none;
            padding: 0.75rem 2rem;
            border-radius: 0.25rem;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s;
            width: 100%;
        }
        
        .submit-btn:hover {
            background-color: #2563eb;
        }
        
        .success-message {
            background-color: #d1fae5;
            color: #065f46;
            padding: 1rem;
            border-radius: 0.25rem;
            margin-top: 1rem;
            display: none;
        }
        
        .success-message.show {
            display: block;
        }
        
        /* Footer */
        footer {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 100%);
            color: white;
            text-align: center;
            padding: 3rem 1.5rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 -4px 20px rgba(0,0,0,0.1);
        }
        
        footer p {
            opacity: 0.9;
            margin: 0.5rem 0;
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes modalSlideIn {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        
        /* Mobile Responsive */
        @media (max-width: 768px) {
            .nav-links {
                position: fixed;
                top: 60px;
                left: -100%;
                width: 100%;
                height: calc(100% - 60px);
                background-color: #1e3a8a;
                flex-direction: column;
                padding: 2rem;
                transition: left 0.3s;
                gap: 1rem;
            }
            
            .nav-links.active {
                left: 0;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero .subtitle {
                font-size: 1.2rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .contact-container {
                grid-template-columns: 1fr;
            }
            
            .profile-photo {
                width: 120px;
                height: 120px;
            }
        }
    </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
  <script src="https://cdn.tailwindcss.com" type="text/javascript"></script>
 </head>
 <body><!-- Navigation -->
  <nav role="navigation" aria-label="Main navigation">
   <div class="nav-container"><button class="mobile-menu-btn" aria-label="Toggle mobile menu" aria-expanded="false">☰</button>
    <ul class="nav-links">
     <li><a href="#home">Home</a></li>
     <li><a href="#about">About</a></li>
     <li><a href="#education">Education</a></li>
     <li><a href="#skills">Skills</a></li>
     <li><a href="#experience">Experience</a></li>
     <li><a href="#achievements">Achievements</a></li>
     <li><a href="#extracurriculars">Extracurriculars</a></li>
     <li><a href="#projects">Projects</a></li>
     <li><a href="#contact">Contact</a></li>
    </ul>
   </div>
  </nav><!-- Hero Section -->
  <header class="hero" id="home">
   <div class="hero-content">
    <div class="avatar" role="img" aria-label="Profile picture of Md. Abdul Fahad"><img src="./phot%20for%20github/Md.%20Abdul%20Fahad.jpg" alt="Md. Abdul Fahad" class="profile-photo" onerror="this.style.display='none'; this.parentElement.innerHTML='<svg width=\'100\' height=\'100\' viewBox=\'0 0 100 100\' fill=\'none\' xmlns=\'http://www.w3.org/2000/svg\'><circle cx=\'50\' cy=\'35\' r=\'20\' fill=\'#1e3a8a\'/><path d=\'M20 85 C20 65, 30 55, 50 55 C70 55, 80 65, 80 85 Z\' fill=\'#1e3a8a\'/></svg>';">
    </div>
    <h1>Md. Abdul Fahad</h1>
    <p class="subtitle">Final-year BBA Student at BAUST</p>
    <p class="location">📍 Nilphamari, Saidpur, Rangpur, Bangladesh</p>
    <div class="cta-text">
     Seeking leadership internship opportunities — Let's connect.
    </div>
    <div class="contact-links"><a href="mailto:mdabdulfahad41@gmail.com" aria-label="Email Md. Abdul Fahad"> 📧 mdabdulfahad41@gmail.com </a> <a href="tel:+8801608216341" aria-label="Call Md. Abdul Fahad"> 📱 +8801608216341 </a> <a href="https://www.linkedin.com/in/md-abdul-fahad" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn profile"> 💼 LinkedIn </a>
    </div>
   </div>
  </header><!-- About Section -->
  <section id="about">
   <h2>About Me</h2>
   <div class="about-content">
    <p>Enthusiastic final-year BBA student at Bangladesh Army University of Science &amp; Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.</p>
   </div>
  </section><!-- Education Section -->
  <section id="education">
   <h2>Education</h2>
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
  </section><!-- Skills Section -->
  <section id="skills">
   <h2>Skills</h2>
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
  </section><!-- Experience Section -->
  <section id="experience">
   <h2>Experience</h2>
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
  </section><!-- Achievements Section -->
  <section id="achievements">
   <h2>Achievements &amp; Training</h2>
   <div class="achievements-grid">
    <article class="achievement-card">
     <div class="achievement-icon">
      📊
     </div>
     <h3>BRAC ISD Excel Training</h3>
     <p>Completed advanced Excel training program focusing on data analysis and visualization techniques</p>
    </article>
    <article class="achievement-card">
     <div class="achievement-icon">
      💼
     </div>
     <h3>BRAC Career Hub Job Readiness Training</h3>
     <p>Enhanced professional skills including resume writing, interview preparation, and workplace communication</p>
    </article>
    <article class="achievement-card">
     <div class="achievement-icon">
      🎮
     </div>
     <h3>Revas Business Simulation</h3>
     <p>Participated in virtual business simulation (May 2025), managing strategic decisions for a travel agency</p>
    </article>
    <article class="achievement-card">
     <div class="achievement-icon">
      🤖
     </div>
     <h3>Agent X AI Competition</h3>
     <p>Competed in AI-focused competition (June 2025), demonstrating innovation and technical problem-solving</p>
    </article>
    <article class="achievement-card">
     <div class="achievement-icon">
      🏆
     </div>
     <h3>Business Case Competition</h3>
     <p>Organized and participated in business case competitions, showcasing analytical and presentation skills</p>
    </article>
    <article class="achievement-card">
     <div class="achievement-icon">
      ⭐
     </div>
     <h3>Best Sub-Leader Award</h3>
     <p>Recognized as Best Sub-Leader in Campus Ambassador Program 2025 for outstanding leadership and performance</p>
    </article>
   </div>
  </section><!-- Extracurriculars Section -->
  <section id="extracurriculars">
   <h2>Leadership &amp; Extracurriculars</h2>
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
  </section><!-- Projects Section -->
  <section id="projects">
   <h2>Projects</h2>
   <div class="projects-grid">
    <article class="project-card" data-project="ebook">
     <div class="project-header">
      <h3>E-book Publishing Platform</h3>
      <p class="project-role">Content Creator &amp; Designer</p>
     </div>
     <div class="project-body">
      <p class="project-description">Managed end-to-end e-book publishing process including content creation, graphic design, and digital distribution for Opportunity Point.</p>
      <div class="project-outcome"><strong>Outcome:</strong> Successfully published multiple e-books with professional layouts and engaging content, reaching diverse audiences
      </div><button class="view-details-btn" aria-label="View details for E-book Publishing Platform project">View Details</button>
     </div>
    </article>
    <article class="project-card" data-project="automation">
     <div class="project-header">
      <h3>Google Forms &amp; AI Automation</h3>
      <p class="project-role">Training Coordinator</p>
     </div>
     <div class="project-body">
      <p class="project-description">Developed and delivered training programs on Google Forms and AI automation tools for BYSDO team members, streamlining data collection and workflow processes.</p>
      <div class="project-outcome"><strong>Outcome:</strong> Improved team efficiency by 40% through automated workflows and reduced manual data entry tasks
      </div><button class="view-details-btn" aria-label="View details for Google Forms &amp; AI Automation project">View Details</button>
     </div>
    </article>
    <article class="project-card" data-project="revas">
     <div class="project-header">
      <h3>Revas Business Simulation</h3>
      <p class="project-role">Strategic Decision Maker</p>
     </div>
     <div class="project-body">
      <p class="project-description">Participated in virtual travel agency simulation, making strategic decisions on pricing, marketing, operations, and resource allocation in a competitive market environment.</p>
      <div class="project-outcome"><strong>Outcome:</strong> Achieved top quartile performance through data-driven decision making and strategic planning
      </div><button class="view-details-btn" aria-label="View details for Revas Business Simulation project">View Details</button>
     </div>
    </article>
   </div>
  </section><!-- Contact Section -->
  <section id="contact">
   <h2>Contact Me</h2>
   <div class="contact-container">
    <div class="contact-info">
     <h3>Get In Touch</h3>
     <div class="contact-item"><span>📧</span> <a href="mailto:mdabdulfahad41@gmail.com">mdabdulfahad41@gmail.com</a>
     </div>
     <div class="contact-item"><span>📱</span> <a href="tel:+8801608216341">+8801608216341</a>
     </div>
     <div class="contact-item"><span>💼</span> <a href="https://www.linkedin.com/in/md-abdul-fahad" target="_blank" rel="noopener noreferrer">linkedin.com/in/md-abdul-fahad</a>
     </div>
     <div class="contact-item"><span>📍</span> <span>Nilphamari, Saidpur, Rangpur, Bangladesh</span>
     </div>
    </div>
   </div>
  </section><!-- Footer -->
  <footer>
   <p>© 2025 Md. Abdul Fahad. All rights reserved.</p>
   <p>Built with passion and dedication</p>
  </footer><!-- Modal -->
  <div class="modal" id="projectModal" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
   <div class="modal-content">
    <div class="modal-header">
     <h3 id="modalTitle"></h3><button class="modal-close" aria-label="Close modal">×</button>
    </div>
    <div class="modal-body" id="modalBody"></div>
   </div>
  </div>
  <script>
        // Configuration object
        const defaultConfig = {
            hero_headline: "Md. Abdul Fahad",
            hero_cta: "Seeking leadership internship opportunities — Let's connect.",
            career_objective: "Enthusiastic final-year BBA student at Bangladesh Army University of Science & Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.",
            email_address: "mdabdulfahad41@gmail.com",
            phone_number: "+8801608216341",
            linkedin_url: "https://www.linkedin.com/in/md-abdul-fahad"
        };

        // Mobile menu toggle
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const navLinks = document.querySelector('.nav-links');

        mobileMenuBtn.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            const isExpanded = navLinks.classList.contains('active');
            mobileMenuBtn.setAttribute('aria-expanded', isExpanded);
        });

        // Close mobile menu when clicking a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileMenuBtn.setAttribute('aria-expanded', 'false');
            });
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                const href = this.getAttribute('href');
                if (href !== '#' && href.startsWith('#')) {
                    e.preventDefault();
                    const target = document.querySelector(href);
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                }
            });
        });

        // Intersection Observer for section animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('section').forEach(section => {
            observer.observe(section);
        });

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
                    
                    <h4>Technologies & Tools</h4>
                    <ul>
                        <li>Canva for graphic design</li>
                        <li>Microsoft Word for content creation</li>
                        <li>Google Workspace for collaboration</li>
                    </ul>
                    
                    <h4>Results & Impact</h4>
                    <ul>
                        <li>Successfully published multiple e-books with professional quality</li>
                        <li>Reached diverse audiences across different platforms</li>
                        <li>Maintained consistent publishing schedule</li>
                        <li>Received positive feedback from readers and stakeholders</li>
                    </ul>
                `
            },
            automation: {
                title: 'Google Forms & AI Automation',
                content: `
                    <h4>Project Overview</h4>
                    <p>Designed and delivered comprehensive training programs on Google Forms and AI automation tools for BYSDO, focusing on improving operational efficiency and data management.</p>
                    
                    <h4>Key Responsibilities</h4>
                    <ul>
                        <li>Developed training curriculum for Google Forms advanced features</li>
                        <li>Implemented AI-powered automation workflows</li>
                        <li>Conducted hands-on training sessions for team members</li>
                        <li>Created documentation and reference materials</li>
                        <li>Provided ongoing technical support and troubleshooting</li>
                    </ul>
                    
                    <h4>Technologies & Tools</h4>
                    <ul>
                        <li>Google Forms for data collection</li>
                        <li>Google Sheets for data processing</li>
                        <li>AI automation tools for workflow optimization</li>
                        <li>Google Apps Script for custom solutions</li>
                    </ul>
                    
                    <h4>Results & Impact</h4>
                    <ul>
                        <li>Improved team efficiency by 40% through automated workflows</li>
                        <li>Reduced manual data entry tasks significantly</li>
                        <li>Enhanced data accuracy and consistency</li>
                        <li>Empowered team members with new technical skills</li>
                    </ul>
                `
            },
            revas: {
                title: 'Revas Business Simulation',
                content: `
                    <h4>Project Overview</h4>
                    <p>Participated in an intensive virtual business simulation managing a travel agency, making strategic decisions across pricing, marketing, operations, and resource allocation in a competitive market environment.</p>
                    
                    <h4>Key Responsibilities</h4>
                    <ul>
                        <li>Analyzed market trends and competitor strategies</li>
                        <li>Developed pricing strategies to maximize profitability</li>
                        <li>Allocated resources efficiently across departments</li>
                        <li>Made data-driven decisions on marketing investments</li>
                        <li>Managed operational costs and service quality</li>
                    </ul>
                    
                    <h4>Skills Demonstrated</h4>
                    <ul>
                        <li>Strategic planning and decision making</li>
                        <li>Financial analysis and budgeting</li>
                        <li>Market analysis and competitive positioning</li>
                        <li>Risk assessment and management</li>
                        <li>Performance monitoring and optimization</li>
                    </ul>
                    
                    <h4>Results & Impact</h4>
                    <ul>
                        <li>Achieved top quartile performance among participants</li>
                        <li>Demonstrated strong analytical and strategic thinking skills</li>
                        <li>Successfully balanced profitability with customer satisfaction</li>
                        <li>Gained practical insights into travel industry operations</li>
                    </ul>
                `
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



        // Element SDK implementation
        async function onConfigChange(config) {
            const heroHeadline = document.querySelector('.hero h1');
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
            emailLinks.forEach(link => {
                link.href = `mailto:${email}`;
            });
            emailDisplays.forEach(display => {
                display.textContent = email;
            });

            const phone = config.phone_number || defaultConfig.phone_number;
            const phoneHref = phone.replace(/\s+/g, '');
            phoneLinks.forEach(link => {
                link.href = `tel:${phoneHref}`;
            });
            phoneDisplays.forEach(display => {
                display.textContent = phone;
            });

            const linkedin = config.linkedin_url || defaultConfig.linkedin_url;
            linkedinLinks.forEach(link => {
                link.href = linkedin;
            });
        }

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
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'99b4de49c1858c28',t:'MTc2MjYwMjc4OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
