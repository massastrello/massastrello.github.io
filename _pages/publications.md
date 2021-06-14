---
layout: page
permalink: /research/
title: research
description: (*) is used to denote equal contribution. Author order determined via coin flips.
years: [2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
