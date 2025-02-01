portfolio-website/
│
├── index.html            # Main HTML file
├── css/
│   └── style.css         # Advanced CSS file for styling
├── js/
│   └── script.js         # Advanced JavaScript file for interactivity
├── images/               # Folder to store images
│   └── profile.jpg       # Example profile image
└── README.md             # Optional file for project documentation
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
/* General Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f0f0f0;
    color: #333;
    line-height: 1.6;
}

/* Header Styling */
header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

/* Section Styling */
section {
    padding: 50px 0;
    background-color: #fff;
}

.container {
    width: 90%;
    margin: 0 auto;
    max-width: 1200px;
}

/* About Section */
.section-about {
    background-color: #e4e4e4;
}

.profile-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.profile-img {
    border-radius: 50%;
    max-width: 200px;
    margin-right: 20px;
}

/* Projects Section */
.section-projects {
    background-color: #f4f4f4;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
}

.project-card {
    background-color: #fff;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.project-card h2 {
    margin-bottom: 15px;
}

.project-link {
    color: #007bff;
    text-decoration: none;
}

/* Contact Form */
.section-contact {
    background-color: #ffffff;
}

form {
    display: flex;
    flex-direction: column;
}

form label {
    margin: 10px 0;
}

form input, form textarea {
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
}

form button {
    background-color: #007bff;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
}

form button:hover {
    background-color: #0056b3;
}

/* Footer Styling */
footer {
    background-color: #333;
    color: white;
    padding: 20px 0;
    text-align: center;
}

/* Responsive Design */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
    }

    .profile-container {
        flex-direction: column;
        align-items: center;
    }

    .projects-grid {
        grid-template-columns: 1fr;
    }
}
// JavaScript for dynamic form submission (Example)

document.getElementById('contact-form').addEventListener('submit', function(e) {
    e.preventDefault();
    
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;
    
    if (email && message) {
        alert('Message Sent! Thank you for contacting me.');
        document.getElementById('contact-form').reset();
    } else {
        alert('Please fill out all fields!');
    }
});

// Example of changing background color when clicking the About section
document.getElementById('about').addEventListener('click', function() {
    document.body.style.backgroundColor = "#d3d3d3";
});
