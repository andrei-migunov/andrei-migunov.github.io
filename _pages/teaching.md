---
layout: page
title: teaching
permalink: /teaching/
description: Courses I've taught or am currently teaching
nav: true
nav_order: 2
display_categories: 
horizontal: false
---

<!-- pages/teaching.md -->
<div class="teaching">
<!-- Display teaching without categories -->
  {%- assign sorted_courses = site.teaching | sort: "semester" -%}
  <!-- Generate cards for each course -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for course in sorted_courses -%}
      {% include teaching_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for course in sorted_courses -%}
      {% include teaching.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>
