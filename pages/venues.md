---
layout: page
show_meta: false
title: "Where to play in Gainesville"
header:
   image_fullwidth: "paddles_at_jtc.jpg"
permalink: "/venues/"
---
<ul>
    {% for post in site.venues %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> ({{ post.short_name }})</li>
    {% endfor %}
</ul>

<h1>When to play</h1>

<p>Scheduled play is available at these times</p>

{% include _whentoplay.html %}

The entire schedule of regular play is also accessible in Google Calendar at [Pickleball in Gainesville, FL](https://calendar.google.com/calendar/embed?height=600&wkst=1&bgcolor=%23ffffff&ctz=America%2FNew_York&src=dDNicXY4MjZiMTUyOWJibWFwbzRwbGYwcmNAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ&color=%23E4C441&showDate=0&showPrint=0&mode=WEEK&title=Pickleball%20in%20Gainesville%2C%20FL&showNav=0&showTabs=0&showCalendars=0&showTz=0){:target="_blank"}

<h1>Open hours</h1>

<p><a href="/venues/northside/">Northside Park</a> is open to the public from 8 a.m. - 11:30 p.m., 7 days a week. It has 4 dedicated, lighted pickleball courts.</p>

<p><a href="/venues/veterans/">Kanapaha Veterans Memorial Park</a> has 6 painted courts open for pickleball Monday - Saturday, 8 a.m. - Noon. </p>

<p><a href="/venues/westside/">Westside Park</a> has three outdoor courts on the east side of the Joyce Oransky Tennis Center outside the fence.</p>
