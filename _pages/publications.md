---
layout: page
permalink: /publications/
title: <i class="fa-regular fa-lightbulb"></i> Research
description:
years: [2025,2024,2022,2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
