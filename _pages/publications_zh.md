---
layout: page
permalink: /zh/publications/
title: 论文
lang: zh
lang_switch: /publications/
description: 按年份倒序排列的论文。
years: [2025, 2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---
<!-- _pages/publications_zh.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
