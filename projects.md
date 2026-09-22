---
layout: page
title: Projects
permalink: /projects/
---

Welcome to my coding portfolio!

## Coding Projects

<ul>
  {% for post in site.posts %}
    {% if post.category == "coding" %}
      <li>
        <strong><a href="{{ post.url }}">{{ post.title }}</a></strong> — <em>{{ post.tech }}</em>
        <p>{{ post.description }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
