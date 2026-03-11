---
layout: page
permalink: /publications/
title: publications
description:
years: [2025, 2023, 2020, 2019, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005, 2004, 2003]
nav: true
nav_order: 4
---

## [Google Scholar](https://scholar.google.com/citations?user=PosEkHAAAAAJ&hl=en)

---
## Selected Peer-Reviewed Articles

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
