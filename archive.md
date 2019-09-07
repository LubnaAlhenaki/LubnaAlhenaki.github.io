---
layout: page
title: Projects
---

<p class="message"> 
 Hey there! This page includes all projects done in the Metis Data Science bootcamp.
</p>

## Blog Posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
