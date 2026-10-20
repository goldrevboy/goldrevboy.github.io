---
layout: default
title: Home
---

I'm a third-year undergraduate in Computer Science and Engineering at
[IIT (BHU) Varanasi](https://iitbhu.ac.in), with a minor in Mathematics,
graduating in June 2027.

I like problems that come with provable guarantees. My current research is in
computational fair division, where I work with
[Prajakta Nimbhorkar](#) <!-- replace # with her homepage URL --> on EFX
allocations and best-of-both-worlds randomization. I'm also interested in using
language design and verification to make distributed programs correct by
construction.

Outside research, I've worked as a quantitative research intern at Quadeye on
mid-frequency trading infrastructure.

## Research interests

- Fair division and computational social choice
- Programming languages and verification
- Distributed systems

## News

<ul class="dated">
{% for item in site.data.news limit: 5 %}
  <li><span class="date">{{ item.date }}</span><span>{{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</span></li>
{% endfor %}
</ul>
