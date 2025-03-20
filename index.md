---
layout: default
title: Home
---

<div class="hero">
  <h1>Hi, I'm <span class="highlight">Felipe</span></h1>
  <p>
    I'm a <span class="highlight">software engineer</span> with a passion for 
    backend development, cloud infrastructure, and automation.
  </p>
  
  <!-- A brief code snippet to showcase your style or favorite snippet -->
  <p>
    Here's a tiny snippet of code I wrote for <code>greeting</code>:
  </p>
  <pre>
    <code>
def greet(name):
    return f"Hello, {name}!"

print(greet("World"))
    </code>
  </pre>
  
  <!-- Some personal "fluff" about your experience -->
  <p>
    Over the years, I've built scalable microservices, automated CI/CD pipelines,
    and collaborated with cross-functional teams to deliver robust products. 
    Outside of work, I tinker with open-source projects and blog about DevOps best practices.
  </p>
</div>

<div class="section">
  <h2>Some of My Old Projects</h2>
  <ul class="card-list">
    <li>
      <strong>Automation Suite</strong>: A Python library that automates server provisioning and
      deployment. <br>
      <a href="https://github.com/your-username/automation-suite">
        View on GitHub
      </a>
    </li>
    <li>
      <strong>Cloud Logger</strong>: A Go-based service for streaming and indexing real-time logs in
      AWS. <br>
      <a href="https://github.com/your-username/cloud-logger">
        View on GitHub
      </a>
    </li>
    <li>
      <strong>Container Monitor</strong>: A Docker-based monitoring tool that
      visualizes resource usage. <br>
      <a href="https://github.com/your-username/container-monitor">
        View on GitHub
      </a>
    </li>
  </ul>
</div>

<div class="section">
  <h2>Recent Posts</h2>
  <ul class="card-list">
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p>Published on {{ post.date | date: "%B %d, %Y" }}</p>
      </li>
    {% endfor %}
  </ul>
  
  <!-- A quick link to view all posts if you have more -->
  <p>
    <a href="/blog" class="highlight">View all posts &raquo;</a>
  </p>
</div>
