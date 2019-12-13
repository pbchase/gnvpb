---
layout: page
show_meta: false
title: "Where to play in Gainesville"
header:
   image_fullwidth: "paddles_at_jtc.jpg"
permalink: "/venues/"
---
<ul>
    {% for post in site.categories.venues %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> ({{ post.short_name }})</li>
    {% endfor %}
</ul>

<h1>When to play</h1>

<p>Scheduled play is available at these times</p>

{% include _whentoplay.html %}
