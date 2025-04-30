# Hello
Welcome to my website 
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background-color: #f4f4f4;
      color: #333;
    }
    header {
      background: #2c3e50;
      color: white;
      padding: 1rem 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav ul {
      display: flex;
      justify-content: center;
      list-style: none;
      padding: 0;
    }
    nav li {
      margin: 0 1rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    .section {
      padding: 4rem 2rem;
      max-width: 1000px;
      margin: auto;
    }
    #about img {
      max-width: 150px;
      border-radius: 50%;
      float: right;
      margin-left: 1rem;
    }
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }
    .project-card {
      background: white;
      padding: 1rem;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .blog-post {
      background: white;
      padding: 1rem;
      margin-bottom: 1rem;
      border-left: 5px solid #3498db;
    }
    form {
      background: white;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    input, textarea {
      padding: 0.75rem;
      font-size: 1rem;
      border-radius: 4px;
      border: 1px solid #ddd;
    }
    button {
      background: #3498db;
      color: white;
      border: none;
      padding: 0.75rem;
      cursor: pointer;
      border-radius: 4px;
      font-size: 1rem;
    }
    footer {
      text-align: center;
      padding: 2rem;
      background: #2c3e50;
      color: white;
    }
    @media (max-width: 600px) {
      nav ul {
        flex-direction: column;
        align-items: center;
      }
      #about img {
        float: none;
        display: block;
        margin: 1rem auto;
      }
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#about">About Me</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="about" class="section">
    <h1>About Me</h1>
    <img src="https://via.placeholder.com/150" alt="Profile Photo" />
    <p>Hello! I'm a web developer passionate about creating modern, responsive websites and applications. With experience in both frontend and backend technologies, I love bringing ideas to life through code.</p>
    <p>When I'm not coding, you'll find me exploring new tech, contributing to open-source projects, or enjoying nature walks.</p>
  </section>

  <section id="projects" class="section">
    <h1>Projects</h1>
    <div class="projects-grid">
      <div class="project-card">
        <h2>Portfolio Website</h2>
        <p>A responsive portfolio template built with HTML/CSS/JS.</p>
        <a href="#">View Project</a>
      </div>
      <div class="project-card">
        <h2>Task Manager App</h2>
        <p>Full-stack React application with MongoDB backend.</p>
        <a href="#">View Project</a>
      </div>
      <div class="project-card">
        <h2>Weather Dashboard</h2>
        <p>Real-time weather data visualization using OpenWeather API.</p>
        <a href="#">View Project</a>
      </div>
    </div>
  </section>

  <section id="blog" class="section">
    <h1>Blog</h1>
    <div class="blog-post">
      <h2>Top 5 JavaScript Frameworks in 2024</h2>
      <p>Exploring the most popular frameworks shaping modern web development...</p>
    </div>
    <div class="blog-post">
      <h2>Responsive Design Principles</h2>
      <p>Understanding fluid layouts, media queries, and mobile-first approach...</p>
    </div>
  </section>

  <section id="contact" class="section">
    <h1>Contact</h1>
    <form>
      <input type="text" placeholder="Your Name" required/>
      <input type="email" placeholder="Your Email" required/>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
      <p id="success-message" style="display:none;">Message sent successfully!</p>
    </form>
  </section>

  <footer>
    &copy; 2024 My Portfolio | Designed & Developed by Me
  </footer>

  <script>
    // Smooth scrolling
    document.querySelectorAll('nav a').forEach(link => {
      link.addEventListener('click', e => {
        e.preventDefault();
        const targetId = link.getAttribute('href');
        document.querySelector(targetId).scrollIntoView({ behavior: 'smooth' });
      });
    });

    // Form submission handling
    document.querySelector('form').addEventListener('submit', e => {
      e.preventDefault();
      document.getElementById('success-message').style.display = 'block';
    });
  </script>
</body>
</html>
```
