<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Housem Moussa - Aerospace Engineer Portfolio</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            background-color: #fff;
            padding: 20px 0;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 24px;
            font-weight: bold;
        }
        .nav-links a {
            margin-left: 20px;
            text-decoration: none;
            color: #333;
        }
        .hero {
            background-color: #f5f5f5;
            text-align: center;
            padding: 100px 0;
        }
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 24px;
            max-width: 600px;
            margin: 0 auto;
        }
        .section {
            padding: 80px 0;
        }
        .section h2 {
            font-size: 36px;
            margin-bottom: 40px;
        }
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        .project {
            background-color: #fff;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            padding: 20px;
            border-radius: 8px;
        }
        .project img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        .contact-form {
            max-width: 500px;
            margin: 0 auto;
        }
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .contact-form button {
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <div class="logo">Housem Moussa</div>
                <div class="nav-links">
                    <a href="#about">About</a>
                    <a href="#projects">Projects</a>
                    <a href="#contact">Contact</a>
                </div>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Innovative Solutions in Engineering and Technology</h1>
            <p>Aerospace Engineer | MEng Graduate | Problem Solver</p>
        </div>
    </section>

    <section id="about" class="section">
        <div class="container">
            <h2>About Me</h2>
            <p>A highly motivated MEng Aerospace Engineering graduate with a strong passion for research and proven skills in independent study. Seeking to pursue a career as a Flight Dynamics Engineer, Systems Engineer, Structural Engineer, or Design Engineer. Bilingual in Italian and Arabic, fluent in English, and a strong command of Spanish.</p>
        </div>
    </section>

    <section id="projects" class="section">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="projects">
                <div class="project">
                    <img src="/api/placeholder/300/200" alt="Aerial Surveillance Drone">
                    <h3>Aerial Surveillance Drone</h3>
                    <p>Engineered a quadrotor drone for ecological research, optimized for capturing high-resolution imagery of remote puffin islands.</p>
                </div>
                <div class="project">
                    <img src="/api/placeholder/300/200" alt="Hydrogen Generation Process">
                    <h3>Hydrogen Generation Process</h3>
                    <p>Developed a sustainable energy solution to power Liverpool John Lennon Airport using wind energy and hydrogen generation.</p>
                </div>
                <div class="project">
                    <img src="/api/placeholder/300/200" alt="ASTOVL Aerodynamics Flight Model">
                    <h3>ASTOVL Aerodynamics Flight Model</h3>
                    <p>Created a comprehensive aerodynamics model and simulation framework for low-speed flight regimes, focusing on transition and hover flight conditions.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="container">
            <h2>Contact Me</h2>
            <form class="contact-form">
                <input type="text" placeholder="Name" required>
                <input type="email" placeholder="Email" required>
                <textarea placeholder="Message" rows="5" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Housem Moussa. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
