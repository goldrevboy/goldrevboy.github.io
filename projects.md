---
layout: default
title: Projects
---

# Projects

<ul class="projects">
{% for p in site.data.projects %}
  <li>
    <span class="proj-name">{% if p.link %}<a href="{{ p.link }}">{{ p.name }}</a>{% else %}{{ p.name }}{% endif %}</span><br>
    {{ p.description }}<br>
    <span class="proj-meta">{{ p.year }}{% if p.tags %} · {{ p.tags | join: ", " }}{% endif %}</span>
  </li>
{% endfor %}
</ul>
