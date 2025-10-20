---
layout: page
title: "Portfolio"
order: 1
icon: fas fa-folder-open
---
<div class="portfolio-section">
  {% for project in site.projects %}
    <div class="portfolio-card" onclick="window.location.href='{{ project.url }}'">
      {% if project.image %}
        <img src="{{ project.image }}" alt="{{ project.title }} image">
      {% endif %}
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
    </div>
  {% endfor %}
</div>

