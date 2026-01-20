---
layout: default
title: Home
---

<div class="theme-toggle-container">
  <button id="theme-toggle" class="theme-toggle-btn" aria-label="Toggle dark mode">
    <span class="theme-icon">🌙</span>
  </button>
</div>

# Peter Nguyen
**Software Engineer | Full Stack Developer | Problem Solver**

<div class="quick-links">
  <a href="#about">About</a> •
  <a href="#experience">Experience</a> •
  <a href="#skills">Skills</a> •
  <a href="#projects">Projects</a> •
  <a href="#blog">Blog</a> •
  <a href="#contact">Contact</a> •
  <a href="/assets/resume.pdf" class="pdf-link">📄 Download Resume</a>
</div>

---

## About Me {#about}

Welcome! I'm a passionate software engineer with expertise in building scalable web applications and solving complex technical challenges. I love creating elegant solutions to difficult problems and continuously learning new technologies.

**Quick Facts:**
- 🎓 Computer Science Background
- 💼 X+ years of professional experience
- 🌍 Based in Australia
- 🚀 Passionate about clean code and best practices

---

## Professional Experience {#experience}

### Senior Software Engineer
**[Company Name]** | *Month Year - Present*

- Led development of [key project/feature] that improved [metric] by X%
- Collaborated with cross-functional teams to deliver high-quality software solutions
- Mentored junior developers and conducted code reviews
- Technologies: [List technologies used]

**Key Achievements:**
- Achieved [specific accomplishment]
- Implemented [important feature/system]
- Optimized [system] resulting in [measurable improvement]

### Software Engineer
**[Company Name]** | *Month Year - Month Year*

- Developed and maintained [type of applications]
- Worked with [technologies/frameworks]
- Contributed to [team achievements]

**Key Achievements:**
- Built [specific feature/project]
- Reduced [metric] by X%
- Improved [system/process]

### [Previous Role]
**[Company Name]** | *Month Year - Month Year*

Brief description of responsibilities and achievements.

---

## Skills & Technologies {#skills}

### Programming Languages
- **Proficient:** Python, JavaScript, TypeScript, Java
- **Familiar:** Go, Ruby, C++

### Frontend Development
- React, Vue.js, Angular
- HTML5, CSS3, SASS/SCSS
- Responsive Design, Accessibility
- Modern JavaScript (ES6+)

### Backend Development
- Node.js, Express, Django, Flask
- RESTful APIs, GraphQL
- Microservices Architecture
- Database Design (SQL & NoSQL)

### DevOps & Tools
- Docker, Kubernetes
- CI/CD (GitHub Actions, Jenkins)
- AWS, Azure, Google Cloud
- Git, Linux/Unix

### Software Engineering
- Agile/Scrum Methodologies
- Test-Driven Development (TDD)
- Design Patterns
- System Design & Architecture

---

## Projects & Portfolio {#projects}

### Project Name One
**[Technologies Used]** | [GitHub](https://github.com/yourusername/project) | [Live Demo](https://project-demo.com)

Description of the project, what problems it solves, and key features you implemented. Highlight interesting technical challenges you overcame.

**Key Features:**
- Feature 1
- Feature 2
- Feature 3

### Project Name Two
**[Technologies Used]** | [GitHub](https://github.com/yourusername/project)

Another project description showcasing your skills and experience.

### Project Name Three
**[Technologies Used]** | [GitHub](https://github.com/yourusername/project)

A third project to demonstrate the breadth of your abilities.

### Open Source Contributions

Brief mention of any open source projects you've contributed to.

---

## Blog {#blog}

I occasionally write about software engineering, technology, and problem-solving. Here are my recent posts:

<div class="blog-list">
{% for post in site.posts limit:5 %}
  <div class="blog-item">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </div>
{% endfor %}
</div>

[View all blog posts →](/blog)

---

## Contact {#contact}

I'm always interested in hearing about new opportunities, collaborations, or just chatting about technology!

**Get in Touch:**
- 📧 Email: [your.email@example.com](mailto:your.email@example.com)
- 💼 LinkedIn: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)
- 🐙 GitHub: [github.com/peternguyen-au](https://github.com/peternguyen-au)
- 🐦 Twitter: [@yourhandle](https://twitter.com/yourhandle)

---

<div class="footer">
  <p>&copy; 2026 Peter Nguyen. Built with Jekyll and hosted on GitHub Pages.</p>
  <p>Last updated: {{ site.time | date: "%B %d, %Y" }}</p>
</div>

<style>
.theme-toggle-container {
  position: fixed;
  top: 20px;
  right: 20px;
  z-index: 1000;
}

.theme-toggle-btn {
  background: var(--bg-secondary, #f5f5f5);
  border: 2px solid var(--border-color, #ddd);
  border-radius: 50%;
  width: 50px;
  height: 50px;
  cursor: pointer;
  font-size: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.theme-toggle-btn:hover {
  transform: scale(1.1);
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.quick-links {
  text-align: center;
  margin: 20px 0;
  font-size: 1.1em;
}

.quick-links a {
  margin: 0 5px;
  text-decoration: none;
}

.pdf-link {
  background: #155799;
  color: white !important;
  padding: 5px 15px;
  border-radius: 5px;
  text-decoration: none;
}

.pdf-link:hover {
  background: #0d3a5f;
}

.blog-list {
  margin: 20px 0;
}

.blog-item {
  margin-bottom: 30px;
  padding-bottom: 20px;
  border-bottom: 1px solid #eee;
}

.blog-item h3 {
  margin-bottom: 5px;
}

.post-date {
  color: #666;
  font-size: 0.9em;
  margin: 5px 0;
}

.footer {
  text-align: center;
  margin-top: 50px;
  padding-top: 20px;
  border-top: 1px solid #eee;
  color: #666;
  font-size: 0.9em;
}

/* Dark mode styles */
body.dark-mode {
  --bg-primary: #1a1a1a;
  --bg-secondary: #2d2d2d;
  --text-primary: #e0e0e0;
  --text-secondary: #b0b0b0;
  --border-color: #444;
  --link-color: #6ab0f3;

  background-color: var(--bg-primary);
  color: var(--text-primary);
}

body.dark-mode .page-header {
  background: linear-gradient(120deg, #1a1a2e, #16213e);
}

body.dark-mode a {
  color: var(--link-color);
}

body.dark-mode .blog-item {
  border-bottom-color: #444;
}

body.dark-mode .footer {
  border-top-color: #444;
  color: var(--text-secondary);
}

body.dark-mode .theme-toggle-btn {
  background: var(--bg-secondary);
  border-color: var(--border-color);
}

body.dark-mode .pdf-link {
  background: #2563eb;
}

body.dark-mode .pdf-link:hover {
  background: #1d4ed8;
}

/* Smooth scroll */
html {
  scroll-behavior: smooth;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .quick-links {
    font-size: 0.9em;
  }

  .theme-toggle-container {
    top: 10px;
    right: 10px;
  }

  .theme-toggle-btn {
    width: 40px;
    height: 40px;
    font-size: 20px;
  }
}
</style>

<script>
// Dark mode toggle functionality
(function() {
  const themeToggle = document.getElementById('theme-toggle');
  const themeIcon = document.querySelector('.theme-icon');
  const body = document.body;

  // Check for saved theme preference or default to light mode
  const currentTheme = localStorage.getItem('theme') || 'light';

  if (currentTheme === 'dark') {
    body.classList.add('dark-mode');
    themeIcon.textContent = '☀️';
  }

  themeToggle.addEventListener('click', function() {
    body.classList.toggle('dark-mode');

    let theme = 'light';
    if (body.classList.contains('dark-mode')) {
      theme = 'dark';
      themeIcon.textContent = '☀️';
    } else {
      themeIcon.textContent = '🌙';
    }

    localStorage.setItem('theme', theme);
  });
})();
</script>
