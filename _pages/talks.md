---
layout: page
permalink: /talk/
title: Talks
description: Talks by categories in reversed chronological order.
years: [2021, 2019, 2018, 2017, 2016]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}
