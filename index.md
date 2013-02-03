---
layout: page
title: Welcome to Gmania's Blog
tagline: 
---
{% include JB/setup %}

### My Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)




