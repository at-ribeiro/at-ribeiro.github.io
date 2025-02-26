---
layout: page
title: "Portfolio"
order: 1
icon: fas fa-folder-open
---

<div class="portfolio-section">
  {% for project in site.projects %}
    <div class="portfolio-card" onclick="window.location.href='{{ project.url }}'" style="cursor: pointer; padding: 20px; border-radius: 8px; transition: transform 0.3s ease, box-shadow 0.3s ease;">
    <style>
      .portfolio-card:hover {
        transform: scale(1.05);
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      }
    </style>
    {% if project.image %}
      <img src="{{ project.image }}" alt="{{ project.title }} image" style="width: 100%; height: auto;">
    {% endif %}
    <h3>{{ project.title }}</h3>
    <p>{{ project.description }}</p>
</div>
  {% endfor %}
</div>