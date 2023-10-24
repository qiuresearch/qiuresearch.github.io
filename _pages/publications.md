---
layout: page
permalink: /publications/
title: publications
description:
years: [2023]
nav: true
nav_order: 4
---


## [Google Scholar](https://scholar.google.com/citations?user=PosEkHAAAAAJ&hl=en)
## [Research Gate](https://www.researchgate.net/profile/Xiangyun-Qiu)

## Selected Peer-Reviewed Articles

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
