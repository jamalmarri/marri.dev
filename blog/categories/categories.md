---
layout: default
title: Categories
permalink: /blog/categories/
---
<div id="categories">
  {% for category in site.categories %}
    <a href="/blog/categories/{{category | first}}/">#{{category | first}}</a><br><br>
  {% endfor %}
</div>
