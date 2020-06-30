---
permalink: /about/
title: "About"
layout: single
author_profile: false
---

The “NYC Response Lab” at Cornell Tech is a joint initiative with CIV:LAB and the NYCEDC to identify community-level COVID-19 related problems and deploy internally-created tech solutions to address them and help New York City people/communities, businesses  and agencies recover from the COVID-19 crisis. We will improve access (to health, mobility, and other resources) and respond in underserved communities in New York using simple and unconventional tools.

# Team
{% assign sorted_team = site.data.team | sort:"first", "last" %}

|:-:|--:|--:|--:|{% for member in sorted_team %}
| ![]({{member.photo}}){: style="height: 100px; border-radius:50%;"} |  {{ member.name }} | {{ member.affiliation }} | <a href="{{member.linkedin}}"><i class="fab fa-linkedin"></i></a>|{% endfor %}
