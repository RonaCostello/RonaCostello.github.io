---
layout: page
permalink: /publications/
title: publications etc.
description: Publications, posters and presentations
years: []
[//]: # Fill in the years to make publications show
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
