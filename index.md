---
layout: default
---

<section class="hero" id="home">
  <span class="hero-greeting">Hi, my name is</span>
  <h1 class="hero-name">David Wong.</h1>
  <h2 class="hero-tagline">I build things with AI.</h2>
  <p class="hero-description">
    I'm a product manager exploring the frontier of AI-assisted development. 
    I use tools like Cursor to rapidly prototype and ship intelligent applications.
  </p>
  <a href="#projects" class="hero-cta">
    View My Work →
  </a>
</section>

<section id="projects">
  <div class="section-header">
    <span class="section-number">01.</span>
    <h2 class="section-title">Projects</h2>
    <div class="section-line"></div>
  </div>
  
  <div class="projects-grid">
    {% for project in site.data.projects %}
    <article class="project-card">
      <div class="project-header">
        <span class="project-icon">{{ project.icon }}</span>
        <div class="project-links">
          {% if project.github and project.github != "" %}
          <a href="{{ project.github }}" target="_blank" rel="noopener" title="GitHub">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
            </svg>
          </a>
          {% endif %}
          {% if project.live and project.live != "" and project.live != "#" %}
          <a href="{{ project.live }}" target="_blank" rel="noopener" title="Live Demo">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
              <polyline points="15 3 21 3 21 9"></polyline>
              <line x1="10" y1="14" x2="21" y2="3"></line>
            </svg>
          </a>
          {% endif %}
        </div>
      </div>
      <h3 class="project-title">{{ project.name }}</h3>
      <p class="project-description">{{ project.description }}</p>
      <div class="project-tags">
        {% for tag in project.tags %}
        <span class="project-tag">{{ tag }}</span>
        {% endfor %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>

<section id="about">
  <div class="section-header">
    <span class="section-number">02.</span>
    <h2 class="section-title">About Me</h2>
    <div class="section-line"></div>
  </div>
  
  <div class="about-content">
    <div class="about-text">
      <p>
        I'm a developer passionate about leveraging <span class="about-highlight">AI-powered tools</span> 
        to accelerate the software development lifecycle. My focus is on building practical applications 
        that solve real problems while exploring the cutting edge of what's possible with AI assistance.
      </p>
      <p>
        I primarily use <span class="about-highlight">Cursor</span> as my AI coding companion, 
        which has transformed how I approach problem-solving and prototyping. From initial concept 
        to production-ready code, I leverage AI to move faster without sacrificing quality.
      </p>
      <p>
        When I'm not coding, I'm usually experimenting with new AI models, contributing to open source, 
        or documenting my learnings to help others navigate this rapidly evolving landscape.
      </p>
    </div>
    <div class="about-image">
      <div class="about-avatar">👨‍💻</div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="section-header">
    <span class="section-number">03.</span>
    <h2 class="section-title">Skills & Tools</h2>
    <div class="section-line"></div>
  </div>
  
  <div class="skills-grid">
    <div class="skill-category">
      <h3 class="skill-category-title">Languages</h3>
      <div class="skill-list">
        <span class="skill-item">Python</span>
        <span class="skill-item">JavaScript</span>
        <span class="skill-item">TypeScript</span>
        <span class="skill-item">Go</span>
        <span class="skill-item">SQL</span>
      </div>
    </div>
    
    <div class="skill-category">
      <h3 class="skill-category-title">Frameworks</h3>
      <div class="skill-list">
        <span class="skill-item">React</span>
        <span class="skill-item">FastAPI</span>
        <span class="skill-item">Node.js</span>
        <span class="skill-item">Next.js</span>
        <span class="skill-item">Flask</span>
      </div>
    </div>
    
    <div class="skill-category">
      <h3 class="skill-category-title">AI & Tools</h3>
      <div class="skill-list">
        <span class="skill-item">Cursor</span>
        <span class="skill-item">OpenAI API</span>
        <span class="skill-item">LangChain</span>
        <span class="skill-item">Claude API</span>
        <span class="skill-item">Hugging Face</span>
      </div>
    </div>
    
    <div class="skill-category">
      <h3 class="skill-category-title">Infrastructure</h3>
      <div class="skill-list">
        <span class="skill-item">Docker</span>
        <span class="skill-item">AWS</span>
        <span class="skill-item">Git</span>
        <span class="skill-item">PostgreSQL</span>
        <span class="skill-item">Redis</span>
      </div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="section-header">
    <span class="section-number">04.</span>
    <h2 class="section-title">Get In Touch</h2>
    <div class="section-line"></div>
  </div>
  
  <div class="contact-content">
    <p class="contact-text">
      I'm always interested in discussing new projects, creative ideas, or opportunities 
      to collaborate on building the future with AI. Feel free to reach out!
    </p>
    
    <div class="contact-links">
      <a href="https://github.com/yourusername" target="_blank" rel="noopener" class="contact-link" title="GitHub">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
        </svg>
      </a>
      <a href="https://linkedin.com/in/yourusername" target="_blank" rel="noopener" class="contact-link" title="LinkedIn">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
          <rect x="2" y="9" width="4" height="12"></rect>
          <circle cx="4" cy="4" r="2"></circle>
        </svg>
      </a>
      <a href="mailto:your.email@example.com" class="contact-link" title="Email">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
          <polyline points="22,6 12,13 2,6"></polyline>
        </svg>
      </a>
    </div>
    
    <a href="mailto:your.email@example.com" class="contact-email">your.email@example.com</a>
  </div>
</section>
