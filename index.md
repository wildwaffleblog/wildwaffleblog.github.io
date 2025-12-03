---
layout: home
title: "BLOG"
---

# Blog

{% for post in site.posts %}
  <article class="post-preview">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%B %-d, %Y" }}</p>

    <div class="post-content">
      {{ post.content }}
    </div>

    <hr>
  </article>
{% endfor %}