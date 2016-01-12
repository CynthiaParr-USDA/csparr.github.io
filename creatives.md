---
layout: page
permalink: /creatives/
title: creatives
description: Creative writing, mostly fiction, some poetry.
---

<ul class="post-list">
{% for creatives in site.creatives reversed %}
    <li>
        <h2><a class="creatives-title" href="{{ creatives.url | prepend: site.baseurl }}">{{ creatives.title }}</a></h2>
        <p class="post-meta">{{ creatives.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
