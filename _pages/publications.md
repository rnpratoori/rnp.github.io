---
layout: page
permalink: /publications/
title: publications
description: 
years_arxiv: [2021, 2020]
years_journals: [2021, 2019, 2018, 2017, 2016, 2015, 2014]
years_conferences: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014]
years_workshops: [2020, 2019, 2018, 2017, 2016]
nav: true
---

## arxiv preprints

<div class="publications">

{% bibliography -f arxiv %}

</div>

## journals

<div class="publications">

{% for y in page.years_journals %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journals -q @*[year={{y}}]* %}
{% endfor %}

</div>


## conferences

<div class="publications">

{% for y in page.years_conferences %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>


## workshops

<div class="publications">


{% for y in page.years_workshops %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshops -q @*[year={{y}}]* %}
{% endfor %}

</div>
