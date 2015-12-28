---
layout: page
permalink: /blog/
title: Blog
description: <!-- Showcase your writing, short stories, or poems. Replace this text with your description. -->
---

<ul class="post-list">
{% for entry in site.blog reversed %}
    <li>
        <h2><a class="poem-title" href="{{ entry.url | prepend: site.baseurl }}">{{ entry.title }}</a></h2>
        <p class="post-meta">{{ entry.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
