---
title: Notebooks
layout: default

notebooks:
  - title: OpenPulse grammar
    url: notebooks/01_openpulse_grammar/openpulse_grammar.html
  - title: Pulse control theory
    url: notebooks/03_pulse_control_theory/pulse_control_theory.html
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
