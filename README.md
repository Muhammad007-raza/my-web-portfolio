<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Interactive Portfolio Website showcasing web development skills.">
    <meta name="author" content="[Your Name]">
    <title>Interactive Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    <header>
        <nav>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#blog">Blog</a></li>
            </ul>
        </nav>
    </header>

    <section id="about" class="section-about">
        <div class="container">
            <h1>About Me</h1>
            <div class="profile-container">
                <img src="images/profile.jpg" alt="Profile picture of [Your Name]" class="profile-img">
                <p>Hi, I am [Your Name], a passionate web developer focusing on creating responsive, user-friendly websites and web applications.</p>
            </div>
        </div>
    </section>

    <section id="projects" class="section-projects">
        <div class="container">
            <h1>My Projects</h1>
            <div class="projects-grid">
                <!-- Example Project -->
                <div class="project-card">
                    <h2>Project 1</h2>
                    <p>Responsive web design project using HTML, CSS, and JavaScript for dynamic interactivity.</p>
                    <a href="https://github.com/your-username/project-1" target="_blank" class="project-link">View on GitHub</a>
                </div>
                <!-- Add more projects as needed -->
            </div>
        </div>
    </section>

    <section id="contact" class="section-contact">
        <div class="container">
            <h1>Contact Me</h1>
            <form id="contact-form" action="#">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required placeholder="Enter your email">
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required placeholder="Your message..."></textarea>
                <button type="submit" class="submit-btn">Send</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 [Your Name]. All rights reserved. <a href="https://github.com/your-username" target="_blank">GitHub</a></p>
    </footer>

    <script src="js/script.js"></script>
</body>
</html>
