---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order. Selected preprints are included.
years: [2026,2025]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->

<div class="pub-note">
This page may not always be up to date. Check my <a rel="external nofollow" href="https://scholar.google.com/citations?hl=en&user=kTNtKRoAAAAJ" target="_blank">Google Scholar profile</a> or <a href="https://www.eurecom.fr/fr/people/wei-fanfu/publications" target="_blank">EURECOM publications</a>.
</div>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
