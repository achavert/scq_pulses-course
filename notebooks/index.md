---
title: Notebooks
---

## Contents

<ul>
{% for page in site.pages %}
  {% if page.path contains 'notebooks/' and page.name endswith '.html' %}
    <li>
      <a href="{{ page.url | relative_url }}">
        {{ page.title | default: page.name }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>
