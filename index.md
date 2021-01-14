---
layout: default
title: A guide to your digital life
---
<div class="listing">
    {% for post in site.posts %}
    <div class="post other link">
      <h2> <a href="{{site.url}}{{post.url}}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date: "%b %-d, %Y" }}</time>
      {{ post.content | strip_html | truncatewords:50 }}
    </div>
    {% endfor %}
</div>
