---
title: /projects
layout: page
permalink: /projects
---

# Projects

<ul>
  {% for post in site.posts %}
    {% if post.tags contains "project" %}
      <li>
        <span>[ {{ post.date | date: "%Y-%m-%d" }} ]</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul> 