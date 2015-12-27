---
layout: page
permalink: /handcraft/
title: Handcraft
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---
<ul class="post-list">
{% for hand in site.handcraft reversed %}
    <li>
        <h2><a class="poem-title" href="{{ hand.url | prepend: site.baseurl }}">{{ hand.title }}</a></h2>
        <p class="post-meta">{{ hand.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
