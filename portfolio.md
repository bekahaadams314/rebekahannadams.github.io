---
layout: page
title: Art
permalink: /art/
---
## Art & Creative Projects

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
  {% for post in site.posts %}
    {% if post.category == "art" %}
      <div style="border: 1px solid #eee; padding: 15px; border-radius: 5px;">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p><strong>Medium:</strong> {{ post.medium }}</p>
        <p>{{ post.description }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>
