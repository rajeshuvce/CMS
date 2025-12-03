---
layout: default
title: Home
---

<section class="hero">
  <h1>Welcome to MS College</h1>
  <p>Excellence in Education, Innovation & Future Learning</p>
  <a href="/about.html" class="btn">Learn More</a>
</section>

<section class="intro">
  <h2>Recent News</h2>
  <ul>
  {% for post in site.posts limit:3 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
  </ul>
</section>

<section class="featured">
  <h2>Courses</h2>
  <ul>
  {% for c in site.courses %}
    <li><a href="{{ c.url }}">{{ c.title }}</a> — {{ c.excerpt }}</li>
  {% endfor %}
  </ul>
</section>
