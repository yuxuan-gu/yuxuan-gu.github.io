---
layout: page
title: activities
permalink: /activities/
description: 
nav: true
nav_order: 3
display_categories: [2022, 2021]
horizontal: false
---

<!-- pages/activities.md -->
<div class="projects">
{% if site.enable_activity_categories and page.display_categories %}
  <!-- Display categorized activities -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_activities = site.activities | where: "category", category %}
  {% assign sorted_activities = categorized_activities | sort: "importance" %}
  <!-- Generate cards for each activity -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
    {% for activity in sorted_activities %}
      {% include activities_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for activity in sorted_activities %}
      {% include activities.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display activities without categories -->

{% assign sorted_activities = site.activities | sort: "importance" %}

  <!-- Generate cards for each activity -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-2">
    {% for activity in sorted_activities %}
      {% include activities_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for activity in sorted_activities %}
      {% include activities.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
