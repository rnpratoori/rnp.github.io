---
layout: page
permalink: /publications/
title: publications
description: 
years_journals: [2023, 2022, 2021, 2020]
years_refconferences: [2017]
years_conferences: [2023, 2022, 2021, 2018, 2017, 2014]
nav: true
---

## Journals

<div class="publications">

{% for y in page.years_journals %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journals -q @*[year={{y}}]* %}
{% endfor %}

</div>


## Refereed Conferences

<div class="publications">

{% for y in page.years_refconferences %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f refconferences -q @*[year={{y}}]* %}
{% endfor %}

</div>


## Other Conferences

<div class="publications">


{% for y in page.years_conferences %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
