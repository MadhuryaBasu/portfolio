<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Madhurya Basu - Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            --secondary-gradient: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            --accent-gradient: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
            --research-gradient: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
            --dark-gradient: linear-gradient(135deg, #2c3e50 0%, #34495e 100%);
            --text-primary: #1a202c;
            --text-secondary: #4a5568;
            --text-light: #718096;
            --bg-primary: #ffffff;
            --bg-secondary: #f7fafc;
            --bg-accent: #edf2f7;
            --shadow-sm: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
            --shadow-md: 0 4px 6px rgba(0,0,0,0.07), 0 2px 4px rgba(0,0,0,0.06);
            --shadow-lg: 0 10px 15px rgba(0,0,0,0.1), 0 4px 6px rgba(0,0,0,0.05);
            --shadow-xl: 0 20px 25px rgba(0,0,0,0.1), 0 10px 10px rgba(0,0,0,0.04);
            --shadow-2xl: 0 25px 50px rgba(0,0,0,0.25);
            --border-radius: 20px;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-primary);
            overflow-x: hidden;
            background: var(--bg-primary);
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--bg-secondary);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary-gradient);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--secondary-gradient);
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            z-index: 1000;
            padding: 1rem 0;
            transition: var(--transition);
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        nav.scrolled {
            background: rgba(255, 255, 255, 0.98);
            box-shadow: var(--shadow-lg);
        }

        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: -0.5px;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2.5rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-primary);
            font-weight: 500;
            font-size: 0.95rem;
            transition: var(--transition);
            position: relative;
            padding: 0.5rem 0;
        }

        .nav-links a:hover {
            color: #667eea;
            transform: translateY(-2px);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background: var(--primary-gradient);
            transition: width 0.3s ease;
            border-radius: 1px;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: var(--primary-gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
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
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><defs><radialGradient id="a" cx="50%" cy="50%" r="50%"><stop offset="0%" stop-color="%23ffffff" stop-opacity="0.1"/><stop offset="100%" stop-color="%23ffffff" stop-opacity="0"/></radialGradient></defs><circle cx="200" cy="200" r="100" fill="url(%23a)"/><circle cx="800" cy="300" r="150" fill="url(%23a)"/><circle cx="400" cy="700" r="120" fill="url(%23a)"/></svg>');
            background-size: cover;
            animation: float 20s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        .hero-particles {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }

        .particle {
            position: absolute;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            animation: particleFloat 8s ease-in-out infinite;
        }

        .particle:nth-child(1) { width: 80px; height: 80px; left: 10%; animation-delay: 0s; }
        .particle:nth-child(2) { width: 60px; height: 60px; left: 20%; animation-delay: 2s; }
        .particle:nth-child(3) { width: 40px; height: 40px; left: 70%; animation-delay: 4s; }
        .particle:nth-child(4) { width: 100px; height: 100px; left: 80%; animation-delay: 1s; }
        .particle:nth-child(5) { width: 50px; height: 50px; left: 60%; animation-delay: 3s; }

        @keyframes particleFloat {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 0.3; }
            50% { transform: translateY(-30px) rotate(180deg); opacity: 0.8; }
        }

        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 1000px;
            padding: 0 2rem;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            padding: 0.5rem 1.5rem;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 500;
            margin-bottom: 2rem;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease 0.2s forwards;
        }

        .hero h1 {
            font-size: 4.5rem;
            font-weight: 900;
            margin-bottom: 1.5rem;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease 0.4s forwards;
            line-height: 1.1;
            letter-spacing: -2px;
        }

        .hero .subtitle {
            font-size: 1.6rem;
            font-weight: 500;
            margin-bottom: 1rem;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease 0.6s forwards;
            color: rgba(255, 255, 255, 0.9);
        }

        .hero .location {
            font-size: 1.2rem;
            font-weight: 400;
            margin-bottom: 3rem;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease 0.8s forwards;
            color: rgba(255, 255, 255, 0.8);
        }

        .hero-buttons {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s ease 1s forwards;
        }

        .cta-button {
            display: inline-block;
            padding: 15px 35px;
            background: rgba(255, 255, 255, 0.2);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1.1rem;
            transition: var(--transition);
            border: 2px solid rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s;
        }

        .cta-button:hover::before {
            left: 100%;
        }

        .cta-button:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
        }

        .cta-secondary {
            background: transparent;
            border: 2px solid rgba(255, 255, 255, 0.5);
        }

        .cta-secondary:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        /* Sections */
        section {
            padding: 120px 0;
            position: relative;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 3.5rem;
            font-weight: 800;
            margin-bottom: 1rem;
            color: var(--text-primary);
            position: relative;
            letter-spacing: -1px;
        }

        .section-subtitle {
            text-align: center;
            font-size: 1.2rem;
            color: var(--text-light);
            margin-bottom: 4rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .section-title::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 4px;
            background: var(--primary-gradient);
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        /* About Section */
        .about {
            background: var(--bg-secondary);
            position: relative;
        }

        .about::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 100px;
            background: linear-gradient(to bottom, transparent, var(--bg-secondary));
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 6rem;
            align-items: center;
        }

        .about-image {
            text-align: center;
            position: relative;
        }

        .about-image::before {
            content: '';
            position: absolute;
            top: -30px;
            left: 50%;
            transform: translateX(-50%);
            width: 320px;
            height: 320px;
            background: var(--primary-gradient);
            border-radius: 50%;
            z-index: -1;
            opacity: 0.1;
            animation: pulse 3s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: translateX(-50%) scale(1); }
            50% { transform: translateX(-50%) scale(1.05); }
        }

        .about-image img {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            object-fit: cover;
            border: 8px solid white;
            box-shadow: var(--shadow-2xl);
            transition: var(--transition);
            position: relative;
            z-index: 1;
        }

        .about-image img:hover {
            transform: scale(1.05);
            box-shadow: 0 30px 60px rgba(0, 0, 0, 0.3);
        }

        .about-text h3 {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            color: var(--text-primary);
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .about-text p {
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 2rem;
            color: var(--text-secondary);
        }

        .about-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin: 3rem 0;
        }

        .stat-item {
            text-align: center;
            padding: 1.5rem;
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-md);
            transition: var(--transition);
        }

        .stat-item:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-xl);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 800;
            background: var(--primary-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: block;
        }

        .stat-label {
            font-size: 0.9rem;
            color: var(--text-light);
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Research Section */
        .research {
            background: var(--bg-primary);
            position: relative;
        }

        .research::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: var(--research-gradient);
            opacity: 0.05;
        }

        .research-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .research-card {
            background: white;
            padding: 3rem;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-md);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .research-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--research-gradient);
        }

        .research-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-2xl);
        }

        .research-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            display: block;
        }

        .research-card h4 {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .research-card p {
            color: var(--text-secondary);
            line-height: 1.6;
            margin-bottom: 1.5rem;
        }

        .research-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .research-tag {
            background: var(--research-gradient);
            color: white;
            padding: 0.3rem 0.8rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* Skills Section */
        .skills {
            background: var(--bg-secondary);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .skill-item {
            background: white;
            padding: 3rem;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-md);
            text-align: center;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .skill-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--primary-gradient);
        }

        .skill-item:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-2xl);
        }

        .skill-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            display: block;
        }

        .skill-item h4 {
            font-size: 1.4rem;
            font-weight: 600;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .skill-item p {
            color: var(--text-secondary);
            margin-bottom: 2rem;
            line-height: 1.6;
        }

        .skill-bar {
            background: #e2e8f0;
            height: 12px;
            border-radius: 6px;
            overflow: hidden;
            margin-top: 1.5rem;
            position: relative;
        }

        .skill-progress {
            height: 100%;
            background: var(--primary-gradient);
            border-radius: 6px;
            width: 0;
            transition: width 2s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
        }

        .skill-progress::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
            animation: shimmer 2s infinite;
        }

        @keyframes shimmer {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }

        /* Projects Section */
        .projects {
            background: var(--bg-primary);
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .project-card {
            background: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow-md);
            transition: var(--transition);
            position: relative;
        }

        .project-card:hover {
            transform: translateY(-15px);
            box-shadow: var(--shadow-2xl);
        }

        .project-image {
            height: 250px;
            background: var(--primary-gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.4rem;
            font-weight: 600;
            position: relative;
            overflow: hidden;
        }

        .project-image::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="%23ffffff20"/><circle cx="80" cy="20" r="2" fill="%23ffffff20"/><circle cx="20" cy="80" r="2" fill="%23ffffff20"/><circle cx="80" cy="80" r="2" fill="%23ffffff20"/><circle cx="50" cy="50" r="2" fill="%23ffffff20"/></svg>');
            background-size: 30px 30px;
            animation: float 10s ease-in-out infinite;
        }

        .project-content {
            padding: 2.5rem;
        }

        .project-content h4 {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .project-content p {
            color: var(--text-secondary);
            margin-bottom: 2rem;
            line-height: 1.6;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 2rem;
        }

        .tech-tag {
            background: var(--bg-secondary);
            color: var(--text-secondary);
            padding: 0.3rem 0.8rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        .project-links {
            display: flex;
            gap: 1rem;
        }

        .project-link {
            padding: 12px 24px;
            background: var(--primary-gradient);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-size: 0.9rem;
            font-weight: 500;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .project-link::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s;
        }

        .project-link:hover::before {
            left: 100%;
        }

        .project-link:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }

        /* Contact Section */
        .contact {
            background: var(--bg-secondary);
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 6rem;
            margin-top: 3rem;
        }

        .contact-info h4 {
            font-size: 1.8rem;
            font-weight: 600;
            margin-bottom: 2rem;
            color: var(--text-primary);
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 2rem;
            padding: 2rem;
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-md);
            transition: var(--transition);
        }

        .contact-item:hover {
            transform: translateX(10px);
            box-shadow: var(--shadow-lg);
        }

        .contact-item i {
            font-size: 1.8rem;
            margin-right: 2rem;
            width: 40px;
            text-align: center;
        }

        .contact-form {
            background: white;
            padding: 3.5rem;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-lg);
        }

        .form-group {
            margin-bottom: 2rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.8rem;
            color: var(--text-primary);
            font-weight: 500;
            font-size: 1rem;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 15px;
            border: 2px solid #e2e8f0;
            border-radius: 10px;
            font-size: 1rem;
            font-family: 'Inter', sans-serif;
            transition: var(--transition);
            background: #f8fafc;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #667eea;
            background: white;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }

        .submit-btn {
            background: var(--primary-gradient);
            color: white;
            padding: 15px 40px;
            border: none;
            border-radius: 25px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            font-family: 'Inter', sans-serif;
            position: relative;
            overflow: hidden;
        }

        .submit-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s;
        }

        .submit-btn:hover::before {
            left: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 15px 35px rgba(102, 126, 234, 0.3);
        }

        /* Footer */
        footer {
            background: var(--dark-gradient);
            color: white;
            text-align: center;
            padding: 4rem 0;
            position: relative;
        }

        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: var(--primary-gradient);
        }

        .social-links {
            margin-bottom: 2rem;
        }

        .social-links a {
            display: inline-block;
            color: white;
            font-size: 2rem;
            margin: 0 1.5rem;
            transition: var(--transition);
            padding: 20px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }

        .social-links a:hover {
            color: #667eea;
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.2);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        /* Animations */
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Loading Animation */
        .loading-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--primary-gradient);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            z-index: 9999;
            transition: opacity 0.5s ease;
        }

        .loading-spinner {
            width: 60px;
            height: 60px;
            border: 4px solid rgba(255, 255, 255, 0.3);
            border-top: 4px solid white;
            border-radius: 50%;
            animation: spin 1s linear infinite;
            margin-bottom: 2rem;
        }

        .loading-text {
            color: white;
            font-size: 1.2rem;
            font-weight: 500;
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 3rem;
            }

            .hero .subtitle {
                font-size: 1.3rem;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
                gap: 4rem;
            }

            .about-stats {
                grid-template-columns: 1fr;
            }

            .contact-content {
                grid-template-columns: 1fr;
                gap: 4rem;
            }

            .section-title {
                font-size: 2.5rem;
            }

            .skills-grid,
            .projects-grid,
            .research-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2.2rem;
            }

            .container {
                padding: 0 1rem;
            }

            section {
                padding: 80px 0;
            }

            .about-image img {
                width: 250px;
                height: 250px;
            }
        }
    </style>
</head>
<body>
    <!-- Loading Overlay -->
    <div class="loading-overlay" id="loading">
        <div class="loading-spinner"></div>
        <div class="loading-text">Loading Portfolio...</div>
    </div>

    <!-- Navigation -->
    <nav id="navbar">
        <div class="nav-container">
            <div class="logo">MADHURYA BASU</div>
            <ul class="nav-links">
                <li><a href="#home">HOME</a></li>
                <li><a href="#about">ABOUT</a></li>
                <li><a href="#research">RESEARCH</a></li>
                <li><a href="#skills">SKILLS</a></li>
                <li><a href="#projects">PROJECTS</a></li>
                <li><a href="#contact">CONTACT</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-particles">
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
            <div class="particle"></div>
        </div>
        <div class="hero-content">
            <div class="hero-badge">🎓 CSE Final Year Student</div>
            <h1>Nice to meet you, I'm Madhurya Basu</h1>
            <p class="subtitle">Frontend Developer • Research Enthusiast • CSE Engineer</p>
            <p class="location">From Kolkata, West Bengal • IEM College</p>
            <div class="hero-buttons">
                <a href="#contact" class="cta-button">Get In Touch</a>
                <a href="#research" class="cta-button cta-secondary">View Research</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title fade-in">About Me</h2>
            <p class="section-subtitle fade-in">Passionate about technology, research, and creating innovative solutions</p>
            <div class="about-content">
                <div class="about-image fade-in">
                    <img src="https://hebbkx1anhila5yf.public.blob.vercel-storage.com/WhatsApp%20Image%202025-06-30%20at%2021.01.41-hKPsBXQaViQE1Ujq26Kk1WaD5sKUMp.jpeg" alt="Madhurya Basu">
                </div>
                <div class="about-text fade-in">
                    <h3>Passionate Engineering Graduate & Research Enthusiast</h3>
                    <p>I'm a B.Tech final year student from IEM Kolkata, specializing in AI domain with a strong foundation in computer science fundamentals. As a research enthusiast, I'm deeply interested in exploring cutting-edge technologies and contributing to academic research in artificial intelligence and machine learning.</p>
                    <p>My academic journey has been marked by excellence - maintaining a CGPA of 8.91 up to 6th semester and ranking among the top 5% of my college in the first year. I combine theoretical knowledge with practical application, always seeking to bridge the gap between research and real-world implementation.</p>
                    
                    <div class="about-stats">
                        <div class="stat-item fade-in">
                            <span class="stat-number">8.91</span>
                            <span class="stat-label">CGPA</span>
                        </div>
                        <div class="stat-item fade-in">
                            <span class="stat-number">Top 5%</span>
                            <span class="stat-label">Class Rank</span>
                        </div>
                        <div class="stat-item fade-in">
                            <span class="stat-number">3+</span>
                            <span class="stat-label">Projects</span>
                        </div>
                    </div>
                    
                    <a href="#contact" class="cta-button">Let's Collaborate</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Research Section -->
    <section id="research" class="research">
        <div class="container">
            <h2 class="section-title fade-in">Research Interests</h2>
            <p class="section-subtitle fade-in">Exploring the frontiers of artificial intelligence and computer science</p>
            <div class="research-grid">
                <div class="research-card fade-in">
                    <div class="research-icon">🤖</div>
                    <h4>Artificial Intelligence</h4>
                    <p>Passionate about machine learning algorithms, neural networks, and their applications in solving real-world problems. Currently exploring deep learning architectures and their optimization techniques.</p>
                    <div class="research-tags">
                        <span class="research-tag">Machine Learning</span>
                        <span class="research-tag">Deep Learning</span>
                        <span class="research-tag">Neural Networks</span>
                    </div>
                </div>
                <div class="research-card fade-in">
                    <div class="research-icon">📊</div>
                    <h4>Data Science & Analytics</h4>
                    <p>Interested in extracting meaningful insights from complex datasets using statistical methods and visualization techniques. Focus on predictive modeling and data-driven decision making.</p>
                    <div class="research-tags">
                        <span class="research-tag">Data Mining</span>
                        <span class="research-tag">Statistical Analysis</span>
                        <span class="research-tag">Predictive Modeling</span>
                    </div>
                </div>
                <div class="research-card fade-in">
                    <div class="research-icon">🔬</div>
                    <h4>Computer Vision</h4>
                    <p>Exploring image processing, pattern recognition, and computer vision applications. Interested in developing systems that can interpret and understand visual information from the world.</p>
                    <div class="research-tags">
                        <span class="research-tag">Image Processing</span>
                        <span class="research-tag">Pattern Recognition</span>
                        <span class="research-tag">OpenCV</span>
                    </div>
                </div>
                <div class="research-card fade-in">
                    <div class="research-icon">🌐</div>
                    <h4>Web Technologies</h4>
                    <p>Research focus on modern web development frameworks, user experience optimization, and progressive web applications. Interested in the intersection of AI and web technologies.</p>
                    <div class="research-tags">
                        <span class="research-tag">Frontend Frameworks</span>
                        <span class="research-tag">UX Research</span>
                        <span class="research-tag">PWA</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills">
        <div class="container">
            <h2 class="section-title fade-in">My Skills</h2>
            <p class="section-subtitle fade-in">A comprehensive toolkit for modern development and research</p>
            <div class="skills-grid">
                <div class="skill-item fade-in">
                    <div class="skill-icon">🌐</div>
                    <h4>Frontend Development</h4>
                    <p>HTML, CSS, JavaScript with modern frameworks and responsive design principles</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="90"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">📊</div>
                    <h4>Data Analysis</h4>
                    <p>Excel, MySQL, PowerBI for comprehensive data analysis and visualization</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="85"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">💻</div>
                    <h4>CS Fundamentals</h4>
                    <p>OOPS, Database Management, Computer Networks, C, C++, Java, DSA, Operating Systems</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="88"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">🔬</div>
                    <h4>Research & Analysis</h4>
                    <p>Academic research methodologies, literature review, data interpretation, and scientific writing</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="82"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">🗣️</div>
                    <h4>Communication & Leadership</h4>
                    <p>Organized TechFest Event (Innovation), led Smart India Hackathon team, started SolarHigh venture</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="85"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">🗄️</div>
                    <h4>Database Management</h4>
                    <p>MySQL, Oracle SQL with advanced query optimization and database design</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="80"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">👨‍💼</div>
                    <h4>Project Management</h4>
                    <p>GitHub, Jira, MS Office Suite with understanding of PM, Scrum Master, and development roles</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="78"></div>
                    </div>
                </div>
                <div class="skill-item fade-in">
                    <div class="skill-icon">🎨</div>
                    <h4>UI/UX Design</h4>
                    <p>Figma, Photoshop with user-centered design principles and prototyping</p>
                    <div class="skill-bar">
                        <div class="skill-progress" data-width="75"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <div class="container">
            <h2 class="section-title fade-in">My Projects</h2>
            <p class="section-subtitle fade-in">Showcasing practical applications of research and development skills</p>
            <div class="projects-grid">
                <div class="project-card fade-in">
                    <div class="project-image">🛒 E-Commerce Platform</div>
                    <div class="project-content">
                        <h4>Amazon Clone</h4>
                        <p>A comprehensive e-commerce platform built with modern web technologies, featuring responsive design, interactive user interface, and optimized performance.</p>
                        <div class="project-tech">
                            <span class="tech-tag">HTML5</span>
                            <span class="tech-tag">CSS3</span>
                            <span class="tech-tag">JavaScript</span>
                            <span class="tech-tag">Responsive Design</span>
                        </div>
                        <div class="project-links">
                            <a href="https://github.com/MadhuryaBasu/amazon-clone/tree/main" class="project-link">Live Demo</a>
                            <a href="https://github.com/MadhuryaBasu/amazon-clone/tree/main" class="project-link">GitHub</a>
                        </div>
                    </div>
                </div>
                <div class="project-card fade-in">
                    <div class="project-image">📊 Data Analysis Project</div>
                    <div class="project-content">
                        <h4>Pizza Sales Analysis</h4>
                        <p>A comprehensive SQL-based data analysis project focusing on pizza sales data with ETL processes, advanced join operations, and business intelligence insights.</p>
                        <div class="project-tech">
                            <span class="tech-tag">SQL</span>
                            <span class="tech-tag">MySQL</span>
                            <span class="tech-tag">Data Analysis</span>
                            <span class="tech-tag">ETL</span>
                        </div>
                        <div class="project-links">
                            <a href="https://github.com/MadhuryaBasu/sql-project" class="project-link">View Project</a>
                            <a href="https://github.com/MadhuryaBasu/sql-project" class="project-link">GitHub</a>
                        </div>
                    </div>
                </div>
                <div class="project-card fade-in">
                    <div class="project-image">🏫 Management System</div>
                    <div class="project-content">
                        <h4>University Management System</h4>
                        <p>A robust university management system implementing object-oriented programming principles with file handling, demonstrating advanced C++ concepts and system design.</p>
                        <div class="project-tech">
                            <span class="tech-tag">C++</span>
                            <span class="tech-tag">OOP</span>
                            <span class="tech-tag">File Handling</span>
                            <span class="tech-tag">System Design</span>
                        </div>
                        <div class="project-links">
                            <a href="https://github.com/MadhuryaBasu/UNIVERSITY-MANAGEMENT-SYSTEM" class="project-link">View Project</a>
                            <a href="https://github.com/MadhuryaBasu/UNIVERSITY-MANAGEMENT-SYSTEM" class="project-link">GitHub</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title fade-in">Get In Touch</h2>
            <p class="section-subtitle fade-in">Let's collaborate on research projects or discuss opportunities</p>
            <div class="contact-content">
                <div class="contact-info fade-in">
                    <h4>Let's Connect</h4>
                    <div class="contact-item">
                        <i>📧</i>
                        <span>madhurya.basu@example.com</span>
                    </div>
                    <div class="contact-item">
                        <i>📱</i>
                        <span>+91 (555) 123-4567</span>
                    </div>
                    <div class="contact-item">
                        <i>📍</i>
                        <span>Kolkata, West Bengal, India</span>
                    </div>
                    <div class="contact-item">
                        <i>🎓</i>
                        <span>IEM College, CSE Final Year</span>
                    </div>
                    <div class="contact-item">
                        <i>💼</i>
                        <span>Available for research collaboration</span>
                    </div>
                </div>
                <form class="contact-form fade-in">
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="subject">Subject</label>
                        <input type="text" id="subject" name="subject" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="submit-btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#" title="GitHub">🐙</a>
                <a href="#" title="LinkedIn">💼</a>
                <a href="#" title="Research Gate">🔬</a>
                <a href="#" title="Twitter">🐦</a>
            </div>
            <p>&copy; 2024 Madhurya Basu. All rights reserved. • Research Enthusiast & Developer</p>
        </div>
    </footer>

    <script>
        // Loading screen
        window.addEventListener('load', function() {
            setTimeout(() => {
                document.getElementById('loading').style.opacity = '0';
                setTimeout(() => {
                    document.getElementById('loading').style.display = 'none';
                }, 500);
            }, 1500);
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
            });
        });

        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // Fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observe all fade-in elements
        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Skill bar animation
        const skillObserver = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const progressBars = entry.target.querySelectorAll('.skill-progress');
                    progressBars.forEach(bar => {
                        const width = bar.getAttribute('data-width');
                        setTimeout(() => {
                            bar.style.width = width + '%';
                        }, 200);
                    });
                }
            });
        }, observerOptions);

        document.querySelectorAll('.skills').forEach(el => {
            skillObserver.observe(el);
        });

        // Contact form submission
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const name = formData.get('name');
            const email = formData.get('email');
            const subject = formData.get('subject');
            const message = formData.get('message');
            
            // Simple validation
            if (!name || !email || !subject || !message) {
                alert('Please fill in all fields.');
                return;
            }
            
            // Simulate form submission
            alert('Thank you for your message! I\'ll get back to you soon.');
            this.reset();
        });

        // Parallax effect for hero section
        window.addEventListener('scroll', function() {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero');
            const rate = scrolled * -0.3;
            
            if (hero && scrolled < window.innerHeight) {
                hero.style.transform = `translateY(${rate}px)`;
            }
        });

        // Add active class to navigation links based on scroll position
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('section[id]');
            const navLinks = document.querySelectorAll('.nav-links a');
            
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if (scrollY >= (sectionTop - 200)) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });

        // Enhanced particle system
        function createParticle() {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.width = (Math.random() * 60 + 20) + 'px';
            particle.style.height = particle.style.width;
            particle.style.animationDuration = (Math.random() * 4 + 4) + 's';
            particle.style.opacity = Math.random() * 0.5 + 0.2;
            document.querySelector('.hero-particles').appendChild(particle);
            
            setTimeout(() => {
                particle.remove();
            }, 8000);
        }

        // Create particles periodically
        setInterval(createParticle, 3000);

        // Counter animation for stats
        function animateCounter(element, target) {
            let current = 0;
            const increment = target / 100;
            const timer = setInterval(() => {
                current += increment;
                if (current >= target) {
                    current = target;
                    clearInterval(timer);
                }
                element.textContent = Math.floor(current);
            }, 20);
        }

        // Trigger counter animation when stats come into view
        const statsObserver = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const statNumber = entry.target.querySelector('.stat-number');
                    const targetValue = parseFloat(statNumber.textContent);
                    if (!isNaN(targetValue)) {
                        animateCounter(statNumber, targetValue);
                    }
                }
            });
        }, { threshold: 0.5 });

        document.querySelectorAll('.stat-item').forEach(el => {
            statsObserver.observe(el);
        });
    </script>
</body>
</html>
