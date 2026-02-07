---
order: 3
layout: page
permalink: /publications/
title: Publications
years: [2026,2025,2024,2023,2021]
nav: true
description: All papers have author names in alphabetical orders.
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
