---
layout: page
title: Publications
permalink: /publications/
years: [ 2023, 2022, 2021, 2020, 2019, 2018, 2009]
---

<div class="publications">


{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f holmgroup -q @*[year={{y}}]* %}
{% endfor %}

