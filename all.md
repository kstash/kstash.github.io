---
title: /all
layout: page
permalink: /all/
---

## All Tags
<ul>
{% for tag in site.tags %}
  <li>{{ tag | first }} ({{ tag | last | size }})</li>
{% endfor %}
</ul>

## All Posts
<ul>
{% for post in site.posts %}
  <li>
    {{ post.title }} - Tags: 
    {% for tag in post.tags %}
      {{ tag }}{% unless forloop.last %}, {% endunless %}
    {% endfor %}
  </li>
{% endfor %}
</ul> 