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

<style>
  .portfolio-section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
  }

  .portfolio-card {
    background: var(--card-bg, #fff);
    color: var(--card-text, #000);
    border-radius: 8px;
    padding: 16px;
    cursor: pointer;
    transition: transform 0.3s ease, box-shadow 0.3s ease, background 0.3s ease;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  }

  .portfolio-card:hover {
    transform: scale(1.05);
    box-shadow: 0 6px 12px rgba(0,0,0,0.2);
  }

  .portfolio-card img {
    width: 100%;
    height: 160px;
    object-fit: cover;
    border-radius: 6px;
    margin-bottom: 10px;
  }

  .portfolio-card h3 {
    margin: 10px 0 6px;
  }

  .portfolio-card p {
    color: inherit;
    font-size: 0.95em;
  }

  /* 🌙 Dark mode support */
  @media (prefers-color-scheme: dark) {
    .portfolio-card {
      background: var(--card-bg-dark, #1e1e1e);
      color: var(--card-text-dark, #f0f0f0);
      box-shadow: 0 2px 8px rgba(255,255,255,0.05);
    }

    .portfolio-card:hover {
      box-shadow: 0 6px 12px rgba(255,255,255,0.1);
    }
  }
</style>


