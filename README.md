<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yashvardhan Singh Hooda - Portfolio</title>
    <meta name="description" content="National-level Shooter | Sports Captain | NDA Aspirant | MUN Winner | Guitarist | Tech Enthusiast" />
    <meta name="author" content="Yashvardhan Singh Hooda" />
    
    <meta property="og:title" content="Yashvardhan Singh Hooda - Portfolio" />
    <meta property="og:description" content="National-level Shooter | Sports Captain | NDA Aspirant | MUN Winner | Guitarist | Tech Enthusiast" />
    <meta property="og:type" content="website" />
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --background: 222.2 84% 4.9%;
            --foreground: 210 40% 98%;
            --card: 222.2 84% 4.9%;
            --card-foreground: 210 40% 98%;
            --popover: 222.2 84% 4.9%;
            --popover-foreground: 210 40% 98%;
            --primary: 217.2 91.2% 59.8%;
            --primary-foreground: 222.2 84% 4.9%;
            --secondary: 217.2 32.6% 17.5%;
            --secondary-foreground: 210 40% 98%;
            --muted: 217.2 32.6% 17.5%;
            --muted-foreground: 215 20.2% 65.1%;
            --accent: 217.2 32.6% 17.5%;
            --accent-foreground: 210 40% 98%;
            --destructive: 0 62.8% 30.6%;
            --destructive-foreground: 210 40% 98%;
            --border: 217.2 32.6% 17.5%;
            --input: 217.2 32.6% 17.5%;
            --ring: 224.3 76.3% 94.0%;
            --radius: 0.75rem;
            --chart-1: 220 70% 50%;
            --chart-2: 160 60% 45%;
            --chart-3: 30 80% 55%;
            --chart-4: 280 65% 60%;
            --chart-5: 340 75% 55%;
            
            /* Custom design tokens */
            --gradient-hero: linear-gradient(135deg, hsl(217.2 91.2% 59.8%) 0%, hsl(280 65% 60%) 50%, hsl(340 75% 55%) 100%);
            --gradient-accent: linear-gradient(135deg, hsl(280 65% 60%) 0%, hsl(340 75% 55%) 100%);
            --gradient-text: linear-gradient(135deg, hsl(186 100% 94%) 0%, hsl(217.2 91.2% 79.8%) 100%);
            --shadow-glow: 0 0 40px hsla(217.2, 91.2%, 59.8%, 0.4);
            --shadow-hover: 0 20px 60px hsla(217.2, 91.2%, 59.8%, 0.3);
            --transition-smooth: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: hsl(var(--background));
            color: hsl(var(--foreground));
            overflow-x: hidden;
            line-height: 1.6;
        }

        /* Hero Section */
        .hero-section {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
            background: var(--gradient-hero);
        }

        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 4xl;
            margin: 0 auto;
            padding: 0 1.5rem;
        }

        .hero-title {
            font-size: clamp(3rem, 8vw, 6rem);
            font-weight: 800;
            margin-bottom: 1.5rem;
            background: var(--gradient-text);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1.1;
        }

        .hero-subtitle {
            font-size: clamp(1rem, 3vw, 1.5rem);
            margin-bottom: 2rem;
            opacity: 0.9;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-button {
            display: inline-block;
            padding: 1rem 2.5rem;
            background: var(--gradient-accent);
            color: white;
            text-decoration: none;
            border-radius: 9999px;
            font-weight: 600;
            font-size: 1.125rem;
            transition: var(--transition-smooth);
            box-shadow: var(--shadow-glow);
        }

        .hero-button:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-hover);
        }

        /* Navigation */
        .navigation {
            position: fixed;
            top: 1.25rem;
            left: 50%;
            transform: translateX(-50%);
            z-index: 1000;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(16px);
            border-radius: 9999px;
            padding: 0.75rem 2rem;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .nav-list {
            list-style: none;
            display: flex;
            gap: 2rem;
            margin: 0;
            padding: 0;
        }

        .nav-button {
            background: none;
            border: none;
            color: hsl(var(--foreground));
            font-weight: 500;
            cursor: pointer;
            transition: var(--transition-smooth);
            font-size: 1rem;
        }

        .nav-button:hover {
            color: hsl(186 100% 94%);
        }

        /* Sections */
        .section {
            padding: 6rem 0;
            position: relative;
        }

        .section-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1.5rem;
        }

        .section-title {
            font-size: clamp(2.5rem, 6vw, 4rem);
            font-weight: 800;
            text-align: center;
            margin-bottom: 4rem;
            background: var(--gradient-text);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        /* Glass effect */
        .glass {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        /* About Section */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            space-y: 1.5rem;
        }

        .about-text p {
            font-size: 1.125rem;
            line-height: 1.75;
            opacity: 0.9;
            margin-bottom: 1.5rem;
        }

        .about-visual {
            text-align: center;
        }

        .profile-card {
            padding: 2.5rem;
            border-radius: 1.5rem;
            transition: var(--transition-smooth);
            transform: perspective(1000px) rotateY(-8deg);
        }

        .profile-card:hover {
            transform: perspective(1000px) rotateY(0deg);
        }

        .profile-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            display: block;
        }

        .profile-title {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: hsl(186 100% 94%);
        }

        /* Achievements Grid */
        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .achievement-card {
            padding: 2rem;
            border-radius: 1rem;
            transition: var(--transition-smooth);
            position: relative;
        }

        .achievement-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }

        .achievement-icon {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            display: block;
        }

        .achievement-title {
            font-size: 1.25rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: hsl(186 100% 94%);
        }

        .achievement-list {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .achievement-list li {
            padding: 0.5rem 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .achievement-list li:last-child {
            border-bottom: none;
        }

        /* Goals Grid */
        .goals-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .goal-card {
            padding: 2rem;
            border-radius: 1rem;
            text-align: center;
            transition: var(--transition-smooth);
        }

        .goal-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }

        .goal-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            display: block;
        }

        .goal-title {
            font-size: 1.25rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: hsl(186 100% 94%);
        }

        .goal-description {
            opacity: 0.9;
            line-height: 1.75;
        }

        /* Contact Section */
        .contact-section {
            background: var(--gradient-hero);
            text-align: center;
        }

        .contact-button {
            display: inline-block;
            padding: 1.25rem 3rem;
            background: var(--gradient-accent);
            color: white;
            text-decoration: none;
            border-radius: 9999px;
            font-weight: 700;
            font-size: 1.25rem;
            transition: var(--transition-smooth);
            box-shadow: var(--shadow-glow);
        }

        .contact-button:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-hover);
        }

        /* Floating Particles */
        .particles-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
            overflow: hidden;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { 
                transform: translateY(0px) rotate(0deg);
                opacity: 0.3;
            }
            50% { 
                transform: translateY(-20px) rotate(180deg);
                opacity: 0.8;
            }
        }

        /* Animations */
        .animate-fade-in-up {
            animation: fadeInUp 1s ease-out forwards;
        }

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

        /* Responsive Design */
        @media (max-width: 768px) {
            .navigation {
                display: none;
            }
            
            .about-grid {
                grid-template-columns: 1fr;
            }
            
            .nav-list {
                gap: 1rem;
            }
            
            .section {
                padding: 4rem 0;
            }
            
            .achievements-grid,
            .goals-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 640px) {
            .hero-button,
            .contact-button {
                padding: 0.875rem 2rem;
                font-size: 1rem;
            }
            
            .achievement-card,
            .goal-card {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Floating Particles -->
    <div class="particles-container" id="particles"></div>

    <!-- Navigation -->
    <nav class="navigation">
        <ul class="nav-list">
            <li>
                <button class="nav-button" onclick="scrollToSection('home')">Home</button>
            </li>
            <li>
                <button class="nav-button" onclick="scrollToSection('about')">About</button>
            </li>
            <li>
                <button class="nav-button" onclick="scrollToSection('achievements')">Achievements</button>
            </li>
            <li>
                <button class="nav-button" onclick="scrollToSection('goals')">Goals</button>
            </li>
            <li>
                <button class="nav-button" onclick="scrollToSection('contact')">Contact</button>
            </li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section">
        <div class="hero-content">
            <h1 class="hero-title">Yashvardhan Singh Hooda</h1>
            <p class="hero-subtitle">
                National-level Shooter | Sports Captain | NDA Aspirant | MUN Winner | Guitarist | Tech Enthusiast
            </p>
            <a href="#about" class="hero-button">Discover My Journey</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <div class="section-container">
            <h2 class="section-title">About Me</h2>
            <div class="about-grid">
                <div class="about-text">
                    <p>
                        I'm Yash, a Class 10 student with a passion for leadership, service, and creativity. As a national-level 10m air pistol shooter and Sports Captain of my school, I've learned the value of discipline, focus, and perseverance.
                    </p>
                    <p>
                        Inspired by my father, who serves in the Indian Air Force, I aim to follow in his footsteps and serve the country with pride through the National Defence Academy. My journey combines the precision of shooting, the creativity of technology, and the harmony of music.
                    </p>
                    <p>
                        When I'm not on the range or studying, you'll find me coding my JARVIS-like AI assistant or playing guitar, finding balance through music and rhythm.
                    </p>
                </div>
                <div class="about-visual">
                    <div class="profile-card glass">
                        <div class="profile-icon">🎯</div>
                        <h3 class="profile-title">Ready to Serve</h3>
                        <p>Following my father's footsteps in the Indian Air Force</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" class="section">
        <div class="section-container">
            <h2 class="section-title">Latest Achievements</h2>
            <div class="achievements-grid">
                <div class="achievement-card glass">
                    <span class="achievement-icon">🔫</span>
                    <h3 class="achievement-title">Shooting Excellence</h3>
                    <ul class="achievement-list">
                        <li>National-level 10m Air Pistol Shooter</li>
                        <li>🥉 3 District-level Medals</li>
                        <li>🏅 Top 10 Shooters of Punjab</li>
                        <li>🇮🇳 Top 50 Shooters in India</li>
                    </ul>
                </div>
                <div class="achievement-card glass">
                    <span class="achievement-icon">🧠</span>
                    <h3 class="achievement-title">Academics & Tech</h3>
                    <ul class="achievement-list">
                        <li>Preparing for National Defence Academy</li>
                        <li>Developing JARVIS-style AI assistant</li>
                        <li>Technology & coding enthusiast</li>
                        <li>Innovation-focused projects</li>
                    </ul>
                </div>
                <div class="achievement-card glass">
                    <span class="achievement-icon">🗣️</span>
                    <h3 class="achievement-title">Leadership & Speaking</h3>
                    <ul class="achievement-list">
                        <li>🏆 3-time MUN Winner</li>
                        <li>🥇 Sports Captain, SHCS</li>
                        <li>Public speaking excellence</li>
                        <li>Student leadership roles</li>
                    </ul>
                </div>
                <div class="achievement-card glass">
                    <span class="achievement-icon">🎸</span>
                    <h3 class="achievement-title">Music & Creativity</h3>
                    <ul class="achievement-list">
                        <li>Passionate Guitarist</li>
                        <li>Regular school performances</li>
                        <li>Personal event appearances</li>
                        <li>Music as balance & expression</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Goals Section -->
    <section id="goals" class="section">
        <div class="section-container">
            <h2 class="section-title">My Goals</h2>
            <div class="goals-grid">
                <div class="goal-card glass">
                    <div class="goal-icon">🎖️</div>
                    <h3 class="goal-title">Military Service</h3>
                    <p class="goal-description">Crack NDA and join the Indian Armed Forces to serve my nation</p>
                </div>
                <div class="goal-card glass">
                    <div class="goal-icon">🏆</div>
                    <h3 class="goal-title">International Shooting</h3>
                    <p class="goal-description">Represent India in national and international shooting competitions</p>
                </div>
                <div class="goal-card glass">
                    <div class="goal-icon">🤖</div>
                    <h3 class="goal-title">AI Innovation</h3>
                    <p class="goal-description">Build real-world AI tools and contribute to technological advancement</p>
                </div>
                <div class="goal-card glass">
                    <div class="goal-icon">✨</div>
                    <h3 class="goal-title">Inspire Others</h3>
                    <p class="goal-description">Motivate others to balance sports, academics, and creativity</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section section">
        <div class="section-container">
            <h2 class="section-title">Let's Connect</h2>
            <p style="font-size: 1.25rem; margin-bottom: 2.5rem; opacity: 0.9;">
                Ready to collaborate or learn more about my journey?
            </p>
            <a href="https://instagram.com/yashvardhan_hooda" target="_blank" rel="noopener noreferrer" class="contact-button">
                📱 Follow on Instagram
            </a>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation
        function scrollToSection(sectionId) {
            const element = document.getElementById(sectionId);
            if (element) {
                element.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }

        // Create floating particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;

            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.top = Math.random() * 100 + '%';
                particle.style.animationDelay = Math.random() * 6 + 's';
                particle.style.animationDuration = (Math.random() * 3 + 3) + 's';
                particlesContainer.appendChild(particle);
            }
        }

        // Parallax effect for hero section
        function handleScroll() {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('#home');
            if (hero) {
                hero.style.transform = `translateY(${scrolled * 0.5}px)`;
            }
        }

        // Intersection Observer for fade-in animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-fade-in-up');
                }
            });
        }, observerOptions);

        // Initialize everything when DOM is loaded
        document.addEventListener('DOMContentLoaded', function() {
            // Create particles
            createParticles();

            // Observe all sections except hero for animations
            const sections = document.querySelectorAll('section:not(#home)');
            sections.forEach(section => {
                observer.observe(section);
            });

            // Add scroll event listener for parallax
            window.addEventListener('scroll', handleScroll);

            // Smooth scrolling for anchor links
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
        });

        // Cleanup on page unload
        window.addEventListener('beforeunload', function() {
            window.removeEventListener('scroll', handleScroll);
            observer.disconnect();
        });
    </script>
</body>
</html>
