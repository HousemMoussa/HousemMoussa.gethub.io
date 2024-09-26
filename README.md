<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Housem Moussa - Aerospace Engineer Portfolio</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
            padding: 1rem;
        }
        .logo {
            float: left;
            font-size: 1.5rem;
            font-weight: bold;
        }
        .nav-links {
            float: right;
        }
        .nav-links a {
            color: #333;
            text-decoration: none;
            padding: 0.5rem 1rem;
        }
        .section {
            padding: 2rem 0;
        }
        .hero {
            background-color: #f4f4f4;
            text-align: center;
            padding: 3rem 0;
        }
        .projects {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .project {
            flex-basis: calc(33.333% - 1rem);
            margin-bottom: 2rem;
            cursor: pointer;
        }
        .project img {
            width: 100%;
            height: auto;
        }
        .project-details {
            display: none;
            background-color: #f4f4f4;
            padding: 1rem;
            margin-top: 1rem;
        }
        .contact-info {
            margin-top: 1rem;
        }
        .contact-info p {
            margin: 0.5rem 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="logo">Housem Moussa</div>
        <div class="nav-links">
            <a href="#about">About</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </div>
    </div>

    <div class="section hero">
        <div class="container">
            <h1>Innovative Solutions in Engineering and Technology</h1>
            <p>Aerospace Engineer | MEng Graduate | Problem Solver</p>
        </div>
    </div>

    <div id="about" class="section">
        <div class="container">
            <h2>About Me</h2>
            <p>A highly motivated MEng Aerospace Engineering graduate with a strong passion for research and proven skills in independent study. Seeking to pursue a career as a Flight Dynamics Engineer, Systems Engineer, Structural Engineer, or Design Engineer. Bilingual in Italian and Arabic, fluent in English, and a strong command of Spanish.</p>
        </div>
    </div>

    <div id="projects" class="section">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="projects">
                <div class="project" onclick="toggleProject('drone')">
                    <img src="/api/placeholder/300/200" alt="Aerial Surveillance Drone">
                    <h3>Aerial Surveillance Drone</h3>
                    <div id="drone" class="project-details">
                        <p>Engineered a quadrotor drone for ecological research, optimized for capturing high-resolution imagery of remote puffin islands. This UAV was designed to conduct precise aerial surveys, quantify cormorant populations, identify nest locations, and monitor population dynamics. The drone's capabilities were enhanced with an integrated GoPro Hero 9 camera for accurate data collection and ecological analysis.</p>
                    </div>
                </div>
                <div class="project" onclick="toggleProject('hydrogen')">
                    <img src="/api/placeholder/300/200" alt="Hydrogen Generation Process">
                    <h3>Hydrogen Generation Process</h3>
                    <div id="hydrogen" class="project-details">
                        <p>Developed a sustainable energy solution to power Liverpool John Lennon Airport using wind energy and hydrogen generation. The project focused on efficient hydrogen production, ensuring year-round energy supply, implementing redundancy planning, and comprehensive airport powering. This innovative approach significantly reduced carbon emissions and successfully integrated with existing renewable energy sources.</p>
                    </div>
                </div>
                <div class="project" onclick="toggleProject('astovl')">
                    <img src="/api/placeholder/300/200" alt="ASTOVL Aerodynamics Flight Model">
                    <h3>ASTOVL Aerodynamics Flight Model</h3>
                    <div id="astovl" class="project-details">
                        <p>Created a comprehensive aerodynamics model and simulation framework for low-speed flight regimes, focusing on transition and hover flight conditions. The project encompassed power-off aerodynamic forces and moments, propulsion system-induced aerodynamic effects, and unpowered in-ground effects. This model enables accurate analysis and prediction of aircraft behavior during critical flight phases, contributing to advanced ASTOVL (Advanced Short Take-Off and Vertical Landing) technology development.</p>
                    </div>
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
                <p>LinkedIn: <a href="https://www.linkedin.com/in/housem-moussa" target="_blank">linkedin.com/in/housem-moussa</a></p>
            </div>
        </div>
    </div>

    <div class="container">
        <p>© 2024 Housem Moussa. All rights reserved.</p>
    </div>

    <script>
        // Smooth scrolling for navigation links
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
        });

        // Toggle project details
        function toggleProject(id) {
            $('#' + id).slideToggle();
        }
    </script>
</body>
</html>
