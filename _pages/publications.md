---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [2021, 2019, 2017, 2014, 2013, 2012, 2011, 2010]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


<!--  <h3 class="year">2018</h3>

W.L. Deng and H. Kesari, <a href='https://www.sciencedirect.com/science/article/pii/S0022509618311281'>Effect of machine stiffness on interpreting contact force--indentation depth curves in adhesive elastic contact experiments</a>, *Journal of the Mechanics and Physics of Solids*, 131:404-423, 2019.
 -->
