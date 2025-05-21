---
layout: default
title: My Portfolio
---

<!-- index.html -->
<h1>👋 Hi, I'm Sridhar Dumbala</h1>
<p>Software Engineer | Finance Tech | HR Tech | Backend Engineering | AI/ML</p>

<h2>📂 Projects</h2>
<div class="projects">
  <div class="card">
    <h3><a href="https://github.com/sridhardumbala/intro_to_nodejs">nodejs learnings</a></h3>
    <p>chat example showcases how to use socket.io with a static express server</p>
  </div>
  <div class="card">
    <h3><a href="https://github.com/sridhardumbala/hello-retail-workshop">Hello, Retail! Nordstrom Technology open-source project</a></h3>
    <p>Hello, Retail! is a 100% serverless, event-driven framework and functional proof-of-concept showcasing a central unified log approach as applied to the retail problem space. All code and patterns are intended to be re-usable for scalable applications large and small.</p>
  </div>
  <div class="card">
    <h3><a href="https://github.com/sridhardumbala/my-journey-with-java">java learnings and build for CLI project</a></h3>
    <p>Command Line Interface application built to mimic basic workflow that can be utilized in car delearships</p>
  </div>
</div>

<h2>📝 Blog</h2>
<ul class="blog-posts">
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: "%b %d, %Y" }}</span> — <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .projects {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1rem;
    margin-top: 1rem;
  }
  .card {
    padding: 1rem;
    border: 1px solid #ddd;
    border-radius: 8px;
    background: #f9f9f9;
    box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.05);
  }
  .blog-posts li {
    margin-bottom: 0.5rem;
  }
</style>
