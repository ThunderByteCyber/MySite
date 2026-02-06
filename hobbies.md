---
layout: page
title: Hobbies & Interests
permalink: /hobbies/
---

{% for hobby in site.hobbies %}
  <h2><a href="{{ hobby.url }}">{{ hobby.title }}</a></h2>
  <p>{{ hobbies.excerpt }}</p>
{% endfor %}

