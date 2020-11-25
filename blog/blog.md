---
layout: default
title: Blog
permalink: /blog/
---
<div id="categories">
  <h3><a href="/blog/categories/">#Categories</a></h3>
</div>

{% for post in site.posts %}
  <div id="post-short">
    <a href="{{post.url}}"><h3>{{post.title}}</h3></a>
    <i>posted on {{post.date | date: "%-d %b %Y"}}</i>
    {% if post.excerpt %}
      {{post.excerpt}}
    {% else %}
      {{post.content}}
    {% endif %}
  </div>
{% endfor %}
