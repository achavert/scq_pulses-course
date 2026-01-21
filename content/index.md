---
title: Notebooks
layout: default

notebooks:
  - title: OpenPulse grammar
    url: content/openpulse_grammar.md
  - title: Pulse control theory
    url: content/pulse_control_theory.html
---

## Contents

<ul>
{% for nb in page.notebooks %}
  <li>
    <a href="{{ nb.url | relative_url }}">
      {{ nb.title }}
    </a>
  </li>
{% endfor %}
</ul>
