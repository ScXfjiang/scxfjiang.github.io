---
layout: page
permalink: /categories/
title: Categories
---

{% for category in site.categories %}
  <h4>{{ category[0] }}</h4>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
