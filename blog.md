---
layout: page
title: Blog
permalink: /blog/
---

Here is my semi-regular blog &#128221;, where I reflect my research or write about stuff which are reletad to my PhD. Eventually other things which cross my mind.

*Chronological* order of all blog posts is below and [category page is here](categories.html)

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
