---
layout: page
title: Tags
permalink: /tags/
published: true
---

<h1>Tags</h1>

<ul>
  {% assign tags = site.tags | sort %}
  {% for tag in tags %}
    {% assign tag_name = tag[0] %}
    <li>
      <a href="#{{ tag_name | slugify }}">{{ tag_name }}</a> ({{ tag[1].size }})
    </li>
  {% endfor %}
</ul>

<hr />

{% for tag in tags %}
  {% assign tag_name = tag[0] %}
  <h2 id="{{ tag_name | slugify }}">{{ tag_name }}</h2>
  <ul>
    {% for post in tag[1] %}
      <li>
        <time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%b %d, %Y' }}</time>
        — <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}

