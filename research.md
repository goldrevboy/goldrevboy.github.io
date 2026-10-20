---
layout: default
title: Research
---

# Research

My interests are in theoretical computer science, mainly **computational social
choice** (fair division, EFX allocations, randomized mechanisms), and in
**programming languages and distributed systems**.

## Papers and preprints

<ol class="pubs">
{% for p in site.data.publications %}
  {% include publication.html p=p %}
{% endfor %}
</ol>

<p class="note">Authors are listed alphabetically, following the convention in theoretical computer science.</p>

## Ongoing work

<!-- Sample descriptions. Rewrite each in one or two sentences of your own. -->

**Best-of-both-worlds fair division.** Randomized allocations that are fair
in expectation (ex-ante) and approximately EFX for every outcome they can
produce (ex-post). With Prajakta Nimbhorkar.

**Hierarchical RL for cloud–fog scheduling.** My bachelor's thesis. See
[Projects](/projects/).
