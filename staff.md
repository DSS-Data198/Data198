---
layout: page
title: Staff
description: Fall 2024 Academic Development
nav_order: 2
---

# Staff
Say HELLO to your Fall 2024 Academic Development Committee! 
{: .no_toc .text-delta }

Hover over some of our icons to get a different side of our personalities!

<!--
<p style="font-size:30px">Note: This page is under construction.</p>


<p style="font-size:30px">Please check back soon for an updated staff roster!</p>

-->


<h2 style="text-align: center;">Executives</h2>

{% assign leads = site.staffers | where: 'role', 'Lead' %}
{% assign sorted_director_by_order = leads | sort: 'order' %}

<div id = "staff-page" class="role flex">
{% for staffer in sorted_director_by_order %}
{{ staffer }}
{% endfor %}
</div>

## Teaching Assistants

{% assign tas = site.staffers | where: 'role', 'TA' %}
{% assign sorted_ta_by_order = tas | sort: 'order' %}

<div id="staff-page" class="role flex">
{% for staffer in sorted_ta_by_order %}
{{ staffer }}
{% endfor %}
</div>

## Tutors

{% assign tutors = site.staffers | where: 'role', 'Tutor' %}

<div id="staff-page" class="role flex">
{% for staffer in tutors %}
{{ staffer }}
{% endfor %}
</div>
