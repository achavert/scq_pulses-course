---
title: Notebooks
layout: default
---

## Contents

<ul>
{% for p in site.pages %}
  {% if p.path contains 'notebooks/' 
        and p.path contains '.html'
        and p.url != '/notebooks/' %}
    <li>
      <a href="{{ p.url | relative_url }}">
        {{ p.title | default: p.name }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>
