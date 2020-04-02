---
layout: page
permalink: /publications/
title: Journals & Conferences
description: A more detailled (and updated) version can be found on <a href="https://scholar.google.fr/citations?user=Hfx_pykAAAAJ&hl=en">Scholar</a>
years: [submitted, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2012, 2011]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
