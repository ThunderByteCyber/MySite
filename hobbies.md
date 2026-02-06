---
layout: hobbies-list
title: Hobbies & Interests
permalink: /hobbies/
---


<div class="columns is-multiline">

{% for hobby in site.hobbies %}
  <div class="column is-4">
    <div class="card">
      {% if hobby.image %}
      <div class="card-image">
        <figure class="image is-16by9">
          <img src="{{ hobby.image }}" alt="{{ hobby.title }}">
        </figure>
      </div>
      {% endif %}

      <div class="card-content">
        <p class="title is-5">
          <a href="{{ hobbies.url }}">{{ hobby.title }}</a>
        </p>
        <p>{{ hobby.excerpt | strip_html | truncate: 120 }}</p>
      </div>
    </div>
  </div>
{% endfor %}

</div>



