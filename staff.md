---
layout: page
title: Staff
description: Fall 2024 Academic Development
#nav_order: 3
---

# Staff
Say HELLO to your Fall 2024 Academic Development Committee! 
{: .no_toc .text-delta }

Hover over some of our icons to get a different side of our personalities!

<!--
<p style="font-size:30px">Note: This page is under construction.</p>


<p style="font-size:30px">Please check back soon for an updated staff roster!</p>

-->


<h2 style="text-align: center;">Course Directors</h2>

{% assign cds = site.staffers | where: 'role', 'CD' %}

<div id = "staff-page" class="role flex">
{% for staffer in cds %}
{{ staffer }}
{% endfor %}
</div>

## Teaching Assistants

{% assign tas = site.staffers | where: 'role', 'TA' %}

<div id="staff-page" class="role flex">
{% for staffer in tas %}
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
