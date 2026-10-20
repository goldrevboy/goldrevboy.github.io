---
layout: default
title: Blog
---

# Blog

Notes, proofs, and things I've learned.
<!-- New posts go in the _posts/ folder. -->

{% assign years = site.posts | group_by_exp: "p", "p.date | date: '%Y'" %}
{% for y in years %}
## {{ y.name }}

<ul class="dated">
{% for post in y.items %}
  <li><span class="date">{{ post.date | date: "%d %b" }}</span><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
{% endfor %}
