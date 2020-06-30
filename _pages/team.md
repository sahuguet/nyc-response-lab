---
permalink: /team/
title: "Our Team"
layout: single
author_profile: false
---

{% assign sorted_team = site.data.team | sort:"first", "last" %}


|:-:|--:|--:|--:|{% for member in sorted_team %}
| ![]({{member.photo}}){: style="height: 100px; border-radius:50%;"} |  {{ member.name }} | {{ member.affiliation }} | <a href="{{member.linkedin}}"><i class="fab fa-linkedin"></i></a>|{% endfor %}
