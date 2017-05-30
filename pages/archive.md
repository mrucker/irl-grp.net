---
layout   : posts
title    : Archive
permalink: /archive/
nav_index: 2 
---

 {% for post in site.posts %}
   
   {% if post.external_url %}
   * [{{post.title}}]({{ post.external_url }})
   {% else %}
   * [{{post.title}}]({{ post.url }})
   {% endif %}

 {% endfor %}
