---
layout: page_bib
title: Publications
permalink: /publications/
description: #Publications and Patents
years: [2023, 2022,2021,2020,2018,2017,2016]
nav: true
nav_order: 2
---
### Publications ###
Go to : [Patents](/publications/#patents)
<div class="publications" id="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},patent=false]*  %}
{% endfor %}
</div>

<hr>

### Patents ###
Go to : [Publications](/publications/#publications)    
<div class="publications" id="patents">
            {% bibliography -f papers -q @*[patent=true]* %}
</div>