---
layout: page
title: Authors
permalink: /authors
---

<ul>
  {% for author in site.authors %}
    <h2><a href="{{ author.website }}">{{ author.name }}</a></h2>
        <h3>{{ author.position }}</h3>
    <li style="display: flex; align-items: flex-start; margin-bottom: 20px;">
      <div style="margin-right: 20px;">
        <img src="assets/img/{{ author.image }}" alt="{{ author.name }}" style="width: 2500px; height: 300px; object-fit: cover;">
      </div>
      <div>
        <p>{{ author.content | markdownify }}</p>
      </div>
    </li>
  {% endfor %}
</ul>