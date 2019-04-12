---
layout: page
permalink: /publications/
title: publications
description: Selective list of publications, categorized by chronological order.
years: [2019, 2018, 2017]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
