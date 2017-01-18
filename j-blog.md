---
layout: page
permalink: /blog/
title: Blog
#description: Writing to share my experience
---

<ul class="post-list">
{% for poem in site.blog reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>