---
layout: page
title: Blog
permalink: /blog/
description: "Daniel Štraub's blog reflecting on his research in transport geography, fare-free public transport, mobility and related topics."
---

This is my semi-regular blog &#128221;. I write here about my research, about things that sit close to it, and occasionally about whatever else crosses my mind.

All posts are listed *chronologically* below. You can also browse them [by category](/categories/).

<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
