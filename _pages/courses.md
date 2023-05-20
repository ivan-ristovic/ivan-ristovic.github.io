---
layout: page
title: Courses
permalink: /courses/
description: 
nav: false
nav_order: 100
display_categories: [Bachelor, Masters, Previous]
---

<!-- pages/courses.md -->
<div class="publications">
  <!-- Display categorized courses -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  <hr/>
  {%- assign categorized_courses = site.courses | where: "category", category -%}
  {%- assign sorted_courses = categorized_courses | sort: "importance" %}
  <!-- Generate cards for each course -->
  <ol class="bibliography">
    <li>
    {%- for course in sorted_courses -%}
      {% include courses.html %}
    {%- endfor %}
    </li>
  </ol>
  {% endfor %}
</div>
