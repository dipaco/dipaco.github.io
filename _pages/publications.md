---
layout: page
permalink: /publications/
title: Publications
description: This is a complete view of my publication record. Please don't hesitate to contact me if you are interested in one of my projects. 
years: [2030, 2029, 2028, 2027, 2026, 2025, 2024, 2023, 2022, 2021, 2020, 2018, 2017, 2015, 2012]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
