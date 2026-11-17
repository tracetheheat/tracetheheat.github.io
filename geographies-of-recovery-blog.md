---
layout: page
title: Geographies of Recovery
permalink: /blog/geographies-of-recovery/
description: "Posts from Geographies of Recovery, Daniel Štraub's blog on addiction treatment and recovery in Poland and Central Europe."
---

Geographies of Recovery is my blog about addiction treatment and recovery in Poland and Central Europe. It accompanies the research project [Geographies of Recovery](/projects/geographies-of-recovery/). Posts are published first on [Substack](https://geographiesofrecovery.substack.com/), where you can also subscribe, and then here on my site.

<ul class="listing">
{% for post in site.categories.GeographiesOfRecovery %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
