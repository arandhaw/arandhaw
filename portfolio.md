---
layout: page
title: Portfolio
---


<div class="portfolio-grid">
  {% for item in site.posts %}
    <div class="portfolio-card">
      <a href="{{ item.url | relative_url }}">
        <h2>{{ item.title }}</h2>
        <p>{{ item.description }}</p>
        {% if item.image %}
          <img src="{{ item.image }}" alt="{{ item.title }}" style="width:200px;height:auto;">
        {% endif %}
      </a>
    </div>
  {% endfor %}
</div>
