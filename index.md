---
layout: default
title: Home
---

<div class="hero">
  <h1>Hi, I'm Felipe</h1>
  <p>I'm a software engineer specializing in backend and DevOps.</p>
</div>

<div class="section">
  <h2>Old Projects</h2>
  <ul class="card-list">
    <li>
      <strong>Project A</strong>: A short description of Project A. 
      <a href="https://github.com/your-username/project-a">View on GitHub</a>
    </li>
    <li>
      <strong>Project B</strong>: A short description of Project B.
      <a href="https://github.com/your-username/project-b">View on GitHub</a>
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
</div>
