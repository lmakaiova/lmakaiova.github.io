---
title: Tréning
layout: category
permalink: "/training/"
---

<ul>
{% assign category_name = "training" %}
{% for post in site.posts %}
  {% if post.categories contains category_name %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%b %-d, %Y" }}</small>
    </li>
  {% endif %}
{% endfor %}
</ul>
