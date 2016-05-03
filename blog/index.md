---
layout: post
title: Grass of Qin's Memory | Blog
css_file: blog
---
{% for post in site.posts_by_language['en'] %}
  <article>
    <div class="article">
      <h1><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }} >></a></h1>
      <div class="excerpt">{{ post.excerpt }}</div>
      <div class="text">{{ post.content | remove: post.excerpt }}</div>
    </div>
    <div class="ext">
      <i class="iconfont">&#xe74e;</i>
      <span>{{ post.date | date_to_string }}</span>
    </div>
  </article>
{% endfor %}

