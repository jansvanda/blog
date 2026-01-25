---
layout: page
title: Trip to the United States of America
permalink: /usa
---

{% assign usa_posts = site.tags.USA | sort: "date" %}

<ul>
  {% for post in usa_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
      <small>({{ post.date | date: "%d.%m.%Y" }})</small>
    </li>
  {% endfor %}
</ul>