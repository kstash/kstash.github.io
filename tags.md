---
title: /tags
layout: page
permalink: /tags/
---

# Tags

<ul>
  {% for tag in site.tags %}
    <ul>
      <a href="{{ "/tags/" | relative_url }}{{ tag[0] | slugify }}/">
        #{{ tag[0] }}</a>({{ tag[1].size }})
    </ul>
  {% endfor %}
</ul>
