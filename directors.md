---
layout: page
title: Previous Directors
description: Contributors to Academic Development over the years!
nav_order: 6
---

# Previous Directors of DATA 198: Introduction to Real World Data Science 
Created by Brandon Lee Concepcion
{: .no_toc .text-delta }

Ever wondered who the previous Directors of Academic Development were? Here they are! 

<!-->
## Website Contributors
{% assign web = site.acknowledgers| where: 'role', 'website' %}
{% assign sorted_website = web | sort: 'rank' %}
-->

<div class="role flex">
{% for acknowledger in sorted_website %}
{{ acknowledger }}
{% endfor %}
</div>


{% assign instructors = site.acknowledgers | where: 'role', 'instructor' %}

<div class="role flex">
{% assign spring2024 = site.acknowledgers | where: 'pronouns', 'Spring 2024' %}
  {% for acknowledger in spring2024 %}
    {{ acknowledger }}
  {% endfor %}
{% assign fall23 = site.acknowledgers | where: 'pronouns', 'Fall 2023' %}
  {% for acknowledger in fall23 %}
    {{ acknowledger }}
  {% endfor %}
{% assign spring2023 = site.acknowledgers | where: 'pronouns', 'Spring 2023' %}
  {% for acknowledger in spring2023 %}
    {{ acknowledger }}
  {% endfor %}
{% assign fall22 = site.acknowledgers | where: 'pronouns', 'Fall 2022' %}
  {% for acknowledger in fall22 %}
    {{ acknowledger }}
  {% endfor %}
{% assign spring2022 = site.acknowledgers | where: 'pronouns', 'Spring 2022' %}
  {% for acknowledger in spring2022 %}
    {{ acknowledger }}
  {% endfor %}
{% assign fall21 = site.acknowledgers | where: 'pronouns', 'Fall 2021' %}
  {% for acknowledger in fall21 %}
    {{ acknowledger }}
  {% endfor %}
</div>

<div class="role flex">
{% assign sp21 = site.acknowledgers | where: 'pronouns', 'Spring 2021' %}
  {% for acknowledger in sp21 %}
    {{ acknowledger }}
  {% endfor %}
{% assign fa20 = site.acknowledgers | where: 'pronouns', 'Fall 2020' %}
  {% for acknowledger in fa20 %}
    {{ acknowledger }}
  {% endfor %}
{% assign sp20 = site.acknowledgers | where: 'pronouns', 'Spring 2020' %}
  {% for acknowledger in sp20 %}
    {{ acknowledger }}
  {% endfor %}
</div>
