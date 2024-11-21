---
layout: page
title: Previous Directors
description: Contributors to Academic Development over the years!
nav_order: 6
---

# Previous Directors of DATA 198: Introduction to Real World Data Science 
Created by Brandon Lee Concepcion
{: .no_toc .text-delta }

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

## Academic Development Directors
{% assign lect = site.acknowledgers| where: 'role', 'instructor' %}

<div class="role flex">
{% for acknowledger in lect %}
{{ acknowledger }}
{% endfor %}
</div>
