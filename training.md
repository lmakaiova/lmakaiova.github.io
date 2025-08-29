---
title: Tréning -tipy ako ....
layout: category
---

Tu bude dačo o tom a potom
<ul>
  {% for post in site.categories.training %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%B %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
