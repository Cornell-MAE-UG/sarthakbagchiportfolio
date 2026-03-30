---
layout: default
title: Sarthak Bagchi - Portfolio
permalink: /projects/
---

## Projects

### Milestone Navigation (ODP)

{% for project in site.projects %}
{% if project.toc == true %}
- [{{ project.title }}]({{ project.url | relative_url }})
{% endif %}
{% endfor %}

---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title }}</p>
        </a>
      </div>
    {% endfor %}
  </div>
</div>