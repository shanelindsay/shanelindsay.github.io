---
layout: page
title: Blog
permalink: /blog/
published: true
lede: Notes on research, teaching, and the tools I use.
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post-card">
      <time class="date" datetime="{{ post.date | date_to_xmlschema }}">Written on {{ post.date | date: "%B %e, %Y" }}</time>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <div class="entry">
        {{ post.excerpt | strip_html | truncate: 200 }}
      </div>
      <a href="{{ post.url | relative_url }}" class="post-nav-link">Read more</a>
    </article>
  {% endfor %}
</div>
