---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
---


# Data 198: Introduction to Real World Data Science <img style = "width: 45px; margin-left: 15px; vertical-align: top;" src = "assets/site_images/dsslogopng.png">

## UC Berkeley, Fall 2024

[Jump to Current Week](#week-{{ site.current_week }}){: .btn .btn-currweek}



<!--

## Instructors For This Week

{% assign instructors = site.staffers | where: 'role', 'presenter' %}

<div class="role flex">
  {% for staffer in instructors %}
  {{ staffer }}
  {% endfor %}
</div>
-->


{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}


{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign active-mods = '' | split: '' %}

{% for mod in mods %}
  {% if mod.status == 'Active' %}
    {% assign active-mods = active-mods | push: mod %}
  {% endif %}
{% endfor %}

{% for module in active-mods %}
  {{ module }}
{% endfor %}