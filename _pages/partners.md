---
permalink: /partners/
title: "Our Partners"
layout: single
author_profile: false
---

{% assign sorted_team = site.data.partners | sort:"name" %}


|:-:|--:|--:|--:|{% for partner in sorted_team %}
| ![]({{partner.image_path}}){: style="height: 100px;"} |  {{ partner.name }} |  | <a href="{{partner.url}}"><i class="fas fa-external-link-alt"></i></a>|{% endfor %}
