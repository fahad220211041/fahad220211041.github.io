<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Md. Abdul Fahad - Final-year BBA student at BAUST seeking leadership internship opportunities. Experienced in business clubs, BNCC, and volunteering.">
  <title>My Design - Md. Abdul Fahad Portfolio</title>
  <script src="/_sdk/element_sdk.js"></script>
  <style>
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
        
        /* Main Header */
        .main-header {
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 100%);
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
            background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 50%, #3b82f6 100%);
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
        
        /* Sections */
        section {
            max-width: 100%;
            width: 100%;
            margin: 0 auto;
            padding: 4rem 3rem;
        }
        
        section:nth-child(even) {
            background-color: white;
        }
        
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
            max-width: 1400px;
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
            max-width: 1400px;
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
            max-width: 1400px;
            margin: 0 auto;
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
            max-width: 1400px;
            margin: 0 auto;
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
            max-width: 1400px;
            margin: 0 auto;
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
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .extracurricular-item {
            background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
            padding: 2rem;
            border-radius: 1rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid rgba(59, 130, 246, 0.1);
        }
        
        .extracurricular-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 30px rgba(59, 130, 246, 0.15);
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
            max-width: 1400px;
            margin: 0 auto;
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
            max-width: 1000px;
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
        
        /* Tablet Responsive */
        @media (max-width: 1024px) {
            .main-header {
                padding: 1.5rem 2rem;
            }
            
            .main-header h1 {
                font-size: 2rem;
            }
            
            section {
                padding: 3rem 2rem;
            }
            
            .hero {
                padding: 4rem 2rem;
            }
            
            .hero h2 {
                font-size: 2.5rem;
            }
            
            .hero .subtitle {
                font-size: 1.3rem;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
            
            .skills-container {
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            }
            
            .projects-grid {
                grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            }
            
            .achievements-grid {
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            }
            
            .extracurricular-list {
                grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            }
        }
        
        /* Mobile Responsive */
        @media (max-width: 768px) {
            .main-header {
                padding: 1.25rem 1.5rem;
            }
            
            .main-header h1 {
                font-size: 1.75rem;
            }
            
            section {
                padding: 2.5rem 1.5rem;
            }
            
            .hero {
                padding: 3rem 1.5rem;
            }
            
            .avatar {
                width: 140px;
                height: 140px;
            }
            
            .profile-photo {
                width: 140px;
                height: 140px;
            }
            
            .hero h2 {
                font-size: 2rem;
            }
            
            .hero .subtitle {
                font-size: 1.2rem;
            }
            
            .hero .location {
                font-size: 1rem;
            }
            
            .cta-text {
                font-size: 1.1rem;
                padding: 1.25rem 2rem;
            }
            
            .contact-links {
                flex-direction: column;
                gap: 1rem;
            }
            
            .section-title {
                font-size: 1.9rem;
                margin-bottom: 2rem;
            }
            
            .about-content {
                font-size: 1rem;
                text-align: left;
            }
            
            .education-item,
            .experience-item {
                padding: 1.75rem;
            }
            
            .experience-header {
                flex-direction: column;
                gap: 0.75rem;
            }
            
            .experience-type {
                align-self: flex-start;
            }
            
            .skills-container {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }
            
            .skill-category {
                padding: 1.75rem;
            }
            
            .skill-list {
                gap: 0.6rem;
            }
            
            .skill-tag {
                padding: 0.55rem 1rem;
                font-size: 0.85rem;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }
            
            .project-header {
                padding: 1.5rem;
            }
            
            .project-body {
                padding: 1.25rem;
            }
            
            .achievements-grid {
                grid-template-columns: 1fr;
                gap: 1.25rem;
            }
            
            .achievement-card {
                padding: 1.5rem;
            }
            
            .extracurricular-list {
                grid-template-columns: 1fr;
                gap: 1.25rem;
            }
            
            .extracurricular-item {
                padding: 1.5rem;
            }
            
            .contact-info {
                padding: 1.75rem;
            }
            
            .contact-item {
                padding: 0.85rem 1rem;
                flex-direction: column;
                align-items: flex-start;
                gap: 0.5rem;
            }
            
            .modal-content {
                margin: 1rem;
                max-height: 85%;
            }
            
            .modal-header {
                padding: 1.5rem;
            }
            
            .modal-body {
                padding: 1.5rem;
            }
            
            footer {
                padding: 2rem 1.5rem;
            }
        }
        
        /* Small Mobile Responsive */
        @media (max-width: 480px) {
            .main-header {
                padding: 1rem 1rem;
            }
            
            .main-header h1 {
                font-size: 1.5rem;
            }
            
            section {
                padding: 2rem 1rem;
            }
            
            .hero {
                padding: 2.5rem 1rem;
            }
            
            .avatar {
                width: 120px;
                height: 120px;
            }
            
            .profile-photo {
                width: 120px;
                height: 120px;
            }
            
            .hero h2 {
                font-size: 1.75rem;
            }
            
            .hero .subtitle {
                font-size: 1.1rem;
            }
            
            .hero .location {
                font-size: 0.95rem;
            }
            
            .cta-text {
                font-size: 1rem;
                padding: 1rem 1.5rem;
            }
            
            .contact-links a {
                font-size: 0.9rem;
                word-break: break-word;
            }
            
            .section-title {
                font-size: 1.6rem;
                margin-bottom: 1.75rem;
            }
            
            .section-title::after {
                width: 80px;
                height: 4px;
            }
            
            .education-item,
            .experience-item,
            .skill-category,
            .achievement-card,
            .extracurricular-item {
                padding: 1.5rem;
            }
            
            .education-item h3,
            .experience-item h3 {
                font-size: 1.3rem;
            }
            
            .skill-category h3 {
                font-size: 1.3rem;
            }
            
            .achievement-card h3 {
                font-size: 1.1rem;
            }
            
            .extracurricular-item h3 {
                font-size: 1.1rem;
            }
            
            .project-header h3 {
                font-size: 1.3rem;
            }
            
            .contact-info {
                padding: 1.5rem;
            }
            
            .contact-item {
                padding: 0.75rem 0.85rem;
            }
            
            .modal-header h3 {
                font-size: 1.3rem;
                padding-right: 2rem;
            }
            
            .modal-body h4 {
                font-size: 1.1rem;
            }
            
            footer {
                padding: 1.75rem 1rem;
                font-size: 0.9rem;
            }
        }
        
        /* Extra Small Mobile */
        @media (max-width: 360px) {
            .main-header h1 {
                font-size: 1.3rem;
            }
            
            .hero h2 {
                font-size: 1.5rem;
            }
            
            .hero .subtitle {
                font-size: 1rem;
            }
            
            .section-title {
                font-size: 1.4rem;
            }
            
            .avatar {
                width: 100px;
                height: 100px;
            }
            
            .profile-photo {
                width: 100px;
                height: 100px;
            }
            
            .cta-text {
                font-size: 0.95rem;
                padding: 0.85rem 1.25rem;
            }
        }

        /* DESIGN gallery styles (added) */
    #design-gallery h1 { text-align:center; color:#1e3a8a; margin-bottom:1rem; font-size:2rem; }
    #design-gallery #info { text-align:center; margin-bottom:1.25rem; color:#334155; font-size:0.95rem; }
    #design-gallery #gallery {
      display:grid;
      grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
      gap: 12px;
      max-width:1200px;
      margin:0 auto;
    }
    #design-gallery #gallery a {
      display:block;
      background:white;
      border-radius:8px;
      overflow:hidden;
      box-shadow: 0 4px 10px rgba(2,6,23,0.06);
      transition: transform .18s, box-shadow .18s;
      text-decoration:none;
    }
    #design-gallery #gallery a:hover { transform: translateY(-6px); box-shadow:0 10px 22px rgba(2,6,23,0.12); }
    #design-gallery #gallery img {
      width:100%;
      height:160px;
      object-fit:cover;
      display:block;
      vertical-align:middle;
    }
    #design-gallery .filename {
      padding:8px 10px;
      font-size:0.87rem;
      color:#1f2937;
      white-space:nowrap;
      overflow:hidden;
      text-overflow:ellipsis;
    }
    #design-gallery #error { color:#b91c1c; text-align:center; margin-top:1rem; }
    #design-gallery footer { text-align:center; margin-top:1.5rem; color:#475569; font-size:0.85rem; }
    @media (max-width:480px){ #design-gallery #gallery img{ height:120px } }
    </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
  <script src="https://cdn.tailwindcss.com" type="text/javascript"></script>
 </head>
 <body><!-- Main Header -->
  <header class="main-header">
   <h1>My Design</h1>
  </header>
  <main class="container"><!-- Hero Section -->
   <section class="hero">
    <div class="hero-content">
     <div class="avatar" role="img" aria-label="Profile picture of Md. Abdul Fahad"><img src="./phot%20for%20github/Md.%20Abdul%20Fahad.jpg" alt="Md. Abdul Fahad" class="profile-photo" onerror="this.style.display='none'; this.parentElement.innerHTML='<svg width=\'100\' height=\'100\' viewBox=\'0 0 100 100\' fill=\'none\' xmlns=\'http://www.w3.org/2000/svg\'><circle cx=\'50\' cy=\'35\' r=\'20\' fill=\'#1e3a8a\'/><path d=\'M20 85 C20 65, 30 55, 50 55 C70 55, 80 65, 80 85 Z\' fill=\'#1e3a8a\'/></svg>';">
     </div>
     <h2>Md. Abdul Fahad</h2>
     <p class="subtitle">Final-year BBA Student at BAUST</p>
     <p class="location">📍 Nilphamari, Saidpur, Rangpur, Bangladesh</p>
     <div class="cta-text">
      Seeking leadership internship opportunities — Let's connect.
     </div>
     <div class="contact-links"><a href="mailto:mdabdulfahad41@gmail.com" aria-label="Email Md. Abdul Fahad"> 📧 mdabdulfahad41@gmail.com </a> <a href="tel:+8801608216341" aria-label="Call Md. Abdul Fahad"> 📱 +8801608216341 </a> <a href="https://www.linkedin.com/in/md-abdul-fahad" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn profile"> 💼 LinkedIn </a>
     </div>
    </div>
   </section><!-- About Section -->
   <section id="about">
    <h2 class="section-title">About Me</h2>
    <div class="about-content">
     <p>Enthusiastic final-year BBA student at Bangladesh Army University of Science &amp; Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.</p>
    </div>
   </section><!-- Education Section -->
   <section id="education">
    <h2 class="section-title">Education</h2>
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
    <h2 class="section-title">Skills</h2>
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
    <h2 class="section-title">Experience</h2>
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
    <h2 class="section-title">Achievements &amp; Training</h2>
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
    <h2 class="section-title">Leadership &amp; Extracurriculars</h2>
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
    <h2 class="section-title">Projects</h2>
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
   </section>

   <!-- DESIGN Gallery Section (added) -->
   <section id="design-gallery">
     <h1>DESIGN Gallery</h1>
     <div id="info">Loading images from /DESIGN/ … (এটি পাবলিক রিপোর জন্য GitHub API ব্যবহার করে)</div>
     <div id="gallery" aria-live="polite"></div>
     <div id="error" role="alert"></div>
     <footer>If some images don't show, try a hard refresh (Ctrl/Cmd+Shift+R). Rate-limit: 60 unauth requests/hour.</footer>
   </section>
   <!-- End DESIGN Gallery Section -->

   <section id="contact">
    <h2 class="section-title">Contact Me</h2>
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
   </section>
  </main><!-- Footer -->
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
            main_heading: "My Design",
            hero_headline: "Md. Abdul Fahad",
            hero_cta: "Seeking leadership internship opportunities — Let's connect.",
            career_objective: "Enthusiastic final-year BBA student at Bangladesh Army University of Science & Technology (BAUST) with active involvement in BNCC, business clubs, and volunteering. Eager to gain practical exposure through leadership internship opportunities and contribute fresh ideas, strong ethics, and a collaborative mindset to a purpose-driven organization.",
            email_address: "mdabdulfahad41@gmail.com",
            phone_number: "+8801608216341",
            linkedin_url: "https://www.linkedin.com/in/md-abdul-fahad"
        };

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
            const mainHeading = document.querySelector('.main-header h1');
            const heroHeadline = document.querySelector('.hero h2');
            const ctaText = document.querySelector('.cta-text');
            const careerObjective = document.querySelector('.about-content p');
            const emailLinks = document.querySelectorAll('a[href^="mailto:"]');
            const phoneLinks = document.querySelectorAll('a[href^="tel:"]');
            const linkedinLinks = document.querySelectorAll('a[href*="linkedin.com"]');
            const emailDisplays = document.querySelectorAll('.contact-links a[href^="mailto:"], .contact-item a[href^="mailto:"]');
            const phoneDisplays = document.querySelectorAll('.contact-links a[href^="tel:"], .contact-item a[href^="tel:"]');

            if (mainHeading) {
                mainHeading.textContent = config.main_heading || defaultConfig.main_heading;
            }

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

  <!-- DESIGN gallery script (added) -->
  <script>
    (async function(){
      // Update owner/repo/path if needed
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
