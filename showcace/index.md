---
layout: page
title: showcase
excerpt: "Instructions on how to install and customize the Jekyll theme So Simple."
modified: 2014-08-08T20:04:41.231140-04:00
image:
  feature: p_sh_index_feature.png
  credit: DreamFactory-Showcase
  creditlink: http://tat306.github.io/DreamFactory/showcase
---

<ul class="post-list">
{% for post in site.categories.showcase %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

