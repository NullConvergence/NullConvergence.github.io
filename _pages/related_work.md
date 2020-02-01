---
layout: page
permalink: /related-work/
title: adversarial-cited
description: A list of publications on the topic of Adversarial Examples I cited over the time. The bib can be found in the repo.
years: [2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2006, 2005, 2004]
---

{% for y in page.years |  reverse %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
