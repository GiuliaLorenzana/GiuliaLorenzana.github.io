---
layout: page
permalink: /talks/
title: Talks
description: Here you can find a complete list of my talks and poster presentations.
years: [Seminars,Contributed talks,Poster]
nav: true
nav_order: 2
---
<!-- _pages/talks.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>
