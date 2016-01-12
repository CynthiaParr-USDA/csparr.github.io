---
layout: page
permalink: /creatives/
title: creatives
description: Creative writing, mostly fiction, some poetry.
---

<ul class="post-list">
{% for poem in site.creatives reversed %}
    <li>
        <h2><a class="work-title" href="{{ work.url | prepend: site.baseurl }}">{{ work.title }}</a></h2>
        <p class="post-meta">{{ work.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
