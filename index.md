---
layout: default
title: 传火祭祀场
---
<div class="listing">
    {% for post in site.posts %}
    <div class="post other link">
        <h2> <a href="{{site.url}}{{post.url}}">{{ post.title }}</a></h2>
        <p class="post-date">{{ post.date | date: "%Y-%m-%d" }}</p>
        <div class="post-content">
          {{ post.content | strip_html | truncatewords:25 }}
          <p class="text-right"><a href="{{ post.url | prepend:site.baseurl }}">Read More &rarr;</a></p>
        </div>
    </div>
    {% endfor %}
</div>
