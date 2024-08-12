---
layout: posts
title: "Two ¢"
permalink: /two-cents/
header:
  image: /assets/images/rr2204_sunset.jpg
---

This is my blog. A place to comment on the world and voice my opinions when then aren't asked for, but I still want to share. It's where I give my two cents, even though two cents won't get you anything en esta economía.

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
      <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
    </li>
  {% endfor %}
</ul>