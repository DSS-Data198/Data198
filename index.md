---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
---


# Data 198: Introduction to Real World Data Science <img style = "width: 45px; margin-left: 15px; vertical-align: top;" src = "assets/site_images/dsslogopng.png">

## UC Berkeley, Fall 2024

<!--
> ### Week 11 Announcements
> - Mid-Semester Feedback Reflection is due **April 22 at 11:59 PM**: [Mid-Semester Feedback Reflection]
> - DeCal Feedback Reflection is due **April 26 at 11:59 PM**: [DeCal Feedback Reflection]
-->

## Announcements
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



[Slides 1]: https://docs.google.com/presentation/d/1NEwKswKvA_Q4dRIW8d_yHcbw16xVDFMM438PY3oswhw/edit?usp=sharing
[Project Checkpoint 0]: https://forms.gle/4XDHXxAdUvyYfUN58

[Slides 2]: https://docs.google.com/presentation/d/1s1KtpZM7-ND4Dl--pGlIR1EWQflIwECVwZCjHWyRzCo/edit?usp=sharing
[Recording]: https://youtu.be/dW2DkGhuw2o
[Pandas Demo I]: https://deepnote.com/workspace/joseph-zhai-4d2cff32-3181-4ae6-a47d-dc9f02262638/project/DSS-Acadev-Lecture-2-Duplicate-82001e9c-93b5-41ef-a966-40cb86c2e838/notebook/Notebook%201-f92f2b9db8e749958ae2ed633fcaf634

[Slides 3]: https://docs.google.com/presentation/d/19-akpz9ImojRjzzXEvBegeiHvkc3MiJCqU5a_bmArAM/edit?usp=sharing
[Pandas Demo II]: https://deepnote.com/workspace/jakex-26b2579d-a0a9-4866-9a6e-9a76f523e999/project/DSS-PANDAS-a79f8a93-a82b-41c3-9849-f96a21636870/notebook/DSS%20PANDAS-f92019557ce44aaaa190e7f7c9c9687a
[Data Cleaning Demo]: https://deepnote.com/workspace/jakex-26b2579d-a0a9-4866-9a6e-9a76f523e999/project/Jake-Xiangs-Untitled-project-b39803e0-90a0-4cea-930e-783d5a994144/notebook/Notebook%201-245e9bebbd374a209f2152cc954b193b
[Pandas Tutor]: https://pandastutor.com/
[Data 100 Lecture Slides]: https://ds100.org/sp24/
[Pandas API Reference]: https://pandas.pydata.org/docs/reference/index.html
[Project Checkpoint 1]: https://bcourses.berkeley.edu/courses/1534410/assignments/8728680

[Slides 4]: https://docs.google.com/presentation/d/1obrS7umyP6wOridZuNJZNr7cLsIA3zGjz-8xNs0GeyA/edit?usp=sharing
[Wilson's Lightning Talk]: https://docs.google.com/presentation/d/1uX7vSRucPcnd4zmqNlyZyspghFSmSINcmHGQZz2kK9s/edit?usp=sharing
[Mini Announcements 4]: https://docs.google.com/presentation/d/16z4DTPUdw0EdIpa8aNCy2grI50p1a1fh2MVd09kLT_Q/edit?usp=sharing
[Data Visualization Demo]: https://deepnote.com/workspace/mitchell-lee-7762986d-0df6-4bbb-aa45-aeaaa1633f9c/project/DSS-Sp23-Lecture-Demo-Data-Viz-EDA-Duplicate-e1110f75-03df-427e-b493-e512c51a282a/notebook/Notebook%201-6b43ab881bf146049ebd07b1a52220d6
[Project Checkpoint 2]: https://bcourses.berkeley.edu/courses/1534410/assignments/8730630

[Slides 5]: https://docs.google.com/presentation/d/1CJONzYWbFoeIzSNrC_gSDgRxkLDkhuRXPcVHi5-C8JE/edit?usp=sharing
[Dhruv's Lightning Talk]: https://docs.google.com/presentation/d/1l924J0UN4NKhd6gDRKKOqKBIzA7nufW6YYdc9crFwOg/edit?usp=sharing
[Mini Announcements 5]: https://docs.google.com/presentation/d/12LPFyRdkmVW22Gj4yaiBVcbG6FUfMMoUNfMaYEVBnrc/edit?usp=sharing
[Project Checkpoint 3]: https://bcourses.berkeley.edu/courses/1534410/assignments/8733701

[Slides 6]: https://docs.google.com/presentation/d/1rB-c0ChkLqgO4EESSD--XQhueuEWiYQ6vrCbbAVz7ck/edit?usp=sharing
[Mini Announcements 6]: https://docs.google.com/presentation/d/1PnBbrMk2rcU-kafg-lz5fZUfly5pv7_tKF3jYPBG6k4/edit?usp=sharing

[Slides 7]: https://docs.google.com/presentation/d/17lZnFMTOM0NZ1v08M3NVKZHPjiWu_l9eGU877-R0C_g/edit?usp=sharing
[Mini Announcements 8]:https://docs.google.com/presentation/d/1weo4p-ebz7sbBFvgTGS-jqOCnPW5_2mF0s4ER8ZRfEg/edit?usp=sharing
[ML Models Demo]: https://deepnote.com/workspace/ryans-workspace-1ba5-0c12a51c-2c5f-47ce-a403-8e829787a597/project/Basic-Machine-Learning-Models-0eb92a08-1222-4b3c-81be-312c63bd701b/notebook/dss-ml-9dede94526244b75a0dd8710525491b0
[Project Checkpoint 4]: https://bcourses.berkeley.edu/courses/1534410/assignments/8736733

[Slides 8]: https://docs.google.com/presentation/d/1oF2vaQIZC-NAs6-7zCamBwECqfMv0H_WdXX86zb3Ts4/edit?usp=sharing
[Jonathan's Lightning Talk]: https://docs.google.com/presentation/d/1mcyHE5bQJY2eRIo28vxuH9JREduxVmcvHIGUEcrt7Pk/edit?usp=sharing
[Mini Announcements 9]: https://docs.google.com/presentation/d/1Y2DIy91rhkFHNQbV2xU3BVZsF9yfydI1hc1MTK7-TNM/edit?usp=sharing
[Model Evaluation Demo]: https://deepnote.com/workspace/bings-workspace-e665b32b-e28f-4b64-afee-8b1d651d83d4/project/DSS-SP23-Decal-Demo-Evaluation-8d2f175b-059c-4e47-b158-93a7100e3305/notebook/demo-f4f13fb3681e4ec2b7b7a8e01b887e20

[Mini Announcements 10]: https://docs.google.com/presentation/d/11QD5sI5Ok6W3JjMH3PbeREYYLa86fSsNnDFsWFghSig/edit?usp=sharing
[Clean Energy Clustering]: https://docs.google.com/presentation/d/1uDLnlq4q5jkZphLFyHSa1jH4bp1G5w3s6cFIdEgHNIs/edit?usp=sharing
[Music Genre Classification]: https://docs.google.com/presentation/d/1o4OTI87XbV8U8Uj2q6MUH5YfXTKIbEYWeYilMcmdUTU/edit?usp=sharing

[Mini Announcements 11]: https://docs.google.com/presentation/d/1MKHeid5RETuocLg9vL-5utZMx1Au0FDFkSJJaibrdoA/edit?usp=sharing
[Mid-Semester Feedback Reflection]: https://forms.gle/mbkt3HP3peiHUN7b7
[DeCal Feedback Reflection]: https://forms.gle/Nocjsy2YsHW74oJfA