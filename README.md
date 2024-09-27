<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Housem Moussa - Aerospace Engineer Portfolio</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <style>
        :root {
            --primary-color: #0a192f;
            --secondary-color: #64ffda;
            --text-color: #8892b0;
            --heading-color: #ccd6f6;
            --background-color: #0a192f;
        }
        
        body {
            font-family: 'Roboto', Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: var(--background-color);
            color: var(--text-color);
        }
        
        .container {
            width: 80%;
            max-width: 1200px;
            margin: auto;
            padding: 0 1rem;
        }
        
        header {
            background-color: rgba(10, 25, 47, 0.9);
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            transition: all 0.3s ease;
            padding: 1rem 0;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--secondary-color);
        }
        
        .nav-links a {
            color: var(--heading-color);
            text-decoration: none;
            padding: 0.5rem 1rem;
            transition: color 0.3s ease;
            font-size: 1.1rem;
        }
        
        .nav-links a:hover {
            color: var(--secondary-color);
        }
        
        .section {
            padding: 6rem 0;
        }
        
        .hero {
            background: linear-gradient(rgba(10, 25, 47, 0.8), rgba(10, 25, 47, 0.8)), url('/api/placeholder/1200/800');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
        }
        
        h1, h2 {
            color: var(--heading-color);
            margin-bottom: 1.5rem;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.4rem;
            margin-bottom: 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: transparent;
            color: var(--secondary-color);
            padding: 0.8rem 2rem;
            border: 2px solid var(--secondary-color);
            border-radius: 5px;
            text-decoration: none;
            transition: all 0.3s ease;
            font-size: 1.1rem;
        }
        
        .btn:hover {
            background-color: rgba(100, 255, 218, 0.1);
            transform: translateY(-3px);
        }
        
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project {
            background-color: rgba(10, 25, 47, 0.5);
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .project:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .project img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project h3 {
            color: var(--heading-color);
            margin-top: 0;
            font-size: 1.4rem;
        }
        
        .contact-info {
            margin-top: 1.5rem;
        }
        
        .contact-info p {
            margin: 0.8rem 0;
            font-size: 1.1rem;
        }
        
        .contact-info a {
            color: var(--secondary-color);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .contact-info a:hover {
            color: var(--heading-color);
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            background-color: rgba(10, 25, 47, 0.5);
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            .hero p {
                font-size: 1.2rem;
            }
            .nav-links {
                display: none;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <div class="logo">HM</div>
            <nav class="nav-links">
                <a href="#about">About</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <div class="hero">
        <div class="container">
            <h1>Housem Moussa</h1>
            <p>Aerospace Engineer | MEng Graduate | Innovator</p>
            <a href="#projects" class="btn">View My Work</a>
        </div>
    </div>

    <div id="about" class="section">
        <div class="container">
            <h2>About Me</h2>
            <p>As a highly motivated MEng Aerospace Engineering graduate, I bring a strong passion for research and proven skills in independent study to the field. My expertise spans Flight Dynamics, Systems Engineering, Structural Engineering, and Design Engineering. With bilingual proficiency in Italian and Arabic, fluency in English, and a strong command of Spanish, I'm well-equipped to contribute to global aerospace projects.</p>
        </div>
    </div>

    <div id="projects" class="section">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="projects">
                <div class="project">
                    <a href="drone-project.html">
                        <img src="/api/placeholder/600/400" alt="Aerial Surveillance Drone">
                        <div class="project-content">
                            <h3>Aerial Surveillance Drone</h3>
                            <p>Engineered a quadrotor drone for ecological research, optimized for capturing high-resolution imagery of remote puffin islands. This UAV conducts precise aerial surveys, quantifies cormorant populations, and monitors population dynamics.</p>
                        </div>
                    </a>
                </div>
                <div class="project">
                    <a href="hydrogen-project.html">
                        <img src="/api/placeholder/600/400" alt="Hydrogen Generation Process">
                        <div class="project-content">
                            <h3>Hydrogen Generation Process</h3>
                            <p>Developed a sustainable energy solution to power Liverpool John Lennon Airport using wind energy and hydrogen generation. This innovative approach significantly reduced carbon emissions and successfully integrated with existing renewable energy sources.</p>
                        </div>
                    </a>
                </div>
                <div class="project">
                    <a href="astovl-project.html">
                        <img src="/api/placeholder/600/400" alt="ASTOVL Aerodynamics Flight Model">
                        <div class="project-content">
                            <h3>ASTOVL Aerodynamics Flight Model</h3>
                            <p>Created a comprehensive aerodynamics model and simulation framework for low-speed flight regimes, focusing on transition and hover flight conditions for Advanced Short Take-Off and Vertical Landing aircraft.</p>
                        </div>
                    </a>
                </div>
            </div>
        </div>
    </div>

    <div id="contact" class="section">
        <div class="container">
            <h2>Contact Me</h2>
            <div class="contact-info">
                <p>Email: <a href="mailto:moussahousem13@gmail.com">moussahousem13@gmail.com</a></p>
                <p>Phone: +44 7429153043</p>
                <p>LinkedIn: <a href="https://www.linkedin.com/in/housem-moussa-63576415a" target="_blank">linkedin.com/in/housem-moussa-63576415a</a></p>
            </div>
        </div>
    </div>

    <footer>
        <div class="container">
            <p>&copy; 2024 Housem Moussa. All rights reserved.</p>
        </div>
    </footer>

    <script>
        $(document).ready(function(){
            $("a").on('click', function(event) {
                if (this.hash !== "") {
                    event.preventDefault();
                    var hash = this.hash;
                    $('html, body').animate({
                        scrollTop: $(hash).offset().top
                    }, 800, function(){
                        window.location.hash = hash;
                    });
                }
            });

            $(window).scroll(function() {
                if ($(this).scrollTop() > 50) {
                    $('header').css('background-color', 'rgba(10, 25, 47, 0.9)');
                } else {
                    $('header').css('background-color', 'transparent');
                }
            });
        });
    </script>
</body>
</html>
