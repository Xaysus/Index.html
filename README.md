<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YOUR ARTIST NAME | Official Portfolio</title>
    <style>
        /* Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #0a0a0a;
            color: #fff;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Navigation */
        .navbar {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(10, 10, 10, 0.95);
            padding: 1rem 2rem;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        .nav-links {
            display: flex;
            justify-content: center;
            list-style: none;
            gap: 3rem;
        }

        .nav-links a {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #ff4444;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(135deg, #1a1a1a 0%, #0a0a0a 100%);
            position: relative;
        }

        .hero-content h1 {
            font-size: 4rem;
            font-weight: 700;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #ff4444, #ffaa00);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-content p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .cta-button {
            display: inline-block;
            padding: 1rem 2rem;
            background: #ff4444;
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: transform 0.3s ease, background 0.3s ease;
        }

        .cta-button:hover {
            transform: translateY(-2px);
            background: #ff3333;
        }

        /* Music Section */
        .music-section {
            padding: 5rem 2rem;
            background: #111;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #ff4444;
        }

        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .track-card {
            background: #1a1a1a;
            border-radius: 15px;
            padding: 1.5rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .track-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(255, 68, 68, 0.3);
        }

        .track-info h3 {
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: #fff;
        }

        .track-info p {
            color: #ccc;
            margin-bottom: 1rem;
        }

        audio {
            width: 100%;
            margin-top: 1rem;
            border-radius: 50px;
        }

        audio::-webkit-media-controls-panel {
            background: #2a2a2a;
        }

        /* About Section */
        .about-section {
            padding: 5rem 2rem;
            background: #0a0a0a;
            text-align: center;
        }

        .about-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .about-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        /* Contact Section */
        .contact-section {
            padding: 5rem 2rem;
            background: #111;
            text-align: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
        }

        .social-link {
            color: #fff;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border: 2px solid #ff4444;
            border-radius: 25px;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background: #ff4444;
            color: #000;
        }

        /* Footer */
        footer {
            background: #0a0a0a;
            padding: 2rem;
            text-align: center;
            color: #666;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.5rem;
            }

            .nav-links {
                gap: 1.5rem;
            }

            .music-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#music">Music</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Xaysus</h1>
            <p>Rapper • Producer • Creative</p>
            <a href="#music" class="cta-button">Listen Now</a>
        </div>
    </section>

    <!-- Music Section -->
    <section id="music" class="music-section">
        <h2 class="section-title">Latest Tracks</h2>
        <div class="music-grid">
            <!-- Track 1 -->
            <div class="track-card">
                <div class="track-info">
                    <h3>Track Title 1</h3>
                    <p>Single • 2024</p>
                    <audio controls>
                        <source src="your-track-1.mp3" type="audio/mpeg">
                        Your browser does not support the audio element.
                    </audio>
                </div>
            </div>

            <!-- Track 2 -->
            <div class="track-card">
                <div class="track-info">
                    <h3>Track Title 2</h3>
                    <p>Single • 2024</p>
                    <audio controls>
                        <source src="your-track-2.mp3" type="audio/mpeg">
                        Your browser does not support the audio element.
                    </audio>
                </div>
            </div>

            <!-- Track 3 -->
            <div class="track-card">
                <div class="track-info">
                    <h3>Track Title 3</h3>
                    <p>Single • 2024</p>
                    <audio controls>
                        <source src="your-track-3.mp3" type="audio/mpeg">
                        Your browser does not support the audio element.
                    </audio>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about-section">
        <h2 class="section-title">About</h2>
        <div class="about-content">
            <p>Write your artist bio here. Talk about your musical journey, influences, and what drives your creativity. This is where you connect with your audience and share your story.</p>
            <p>Include your achievements, collaborations, or anything else that defines your artistic identity.</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <h2 class="section-title">Connect With Me</h2>
        <div class="social-links">
            <a href="#" class="social-link">Spotify</a>
            <a href="#" class="social-link">Instagram</a>
            <a href="#" class="social-link">YouTube</a>
            <a href="#" class="social-link">SoundCloud</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 YOUR ARTIST NAME. All rights reserved.</p>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Add scroll effect to navbar
        window.addEventListener('scroll', function() {
            const navbar = document.querySelector('.navbar');
            if (window.scrollY > 100) {
                navbar.style.background = 'rgba(10, 10, 10, 0.98)';
            } else {
                navbar.style.background = 'rgba(10, 10, 10, 0.95)';
            }
        });
    </script>
</body>
</html>
