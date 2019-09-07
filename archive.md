---
layout: page
title: Projects
---

<p class="message"> 
 Hey there! This page includes all projects done in the Metis Data Science bootcamp.
</p>

## Projects Posts

{% for post in site.posts %}
  * [ {{ post.title }} ]({{ post.url }})
{% endfor %}
