---
layout: page
permalink: /publications/
title: publications
description: An up-to-date list is available on <i class="fas fa-hashtag fa-sm"></i><a href='https://scholar.google.com/citations?user=Kk2l14wAAAAJ&hl'>Google Scholar</a>.
years: [2020, 2022, 2023]
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
