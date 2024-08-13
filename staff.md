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


<h2 style="text-align: center;">Leads</h2>

{% assign leads = site.staffers | where: 'role', 'Lead' %}

<div id = "staff-page" class="role flex">
{% for staffer in leads %}
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

<p style="font-size:20px">Please check back soon for an updated tutor roster!</p>

{% assign tutors = site.staffers | where: 'role', 'Tutor' %}

<div id="staff-page" class="role flex">
{% for staffer in tutors %}
{{ staffer }}
{% endfor %}
</div>
