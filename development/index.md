---
layout: page
title: development
excerpt: "Progression of this project"
search_omit: true
image:
  feature: p_d_index_feature.png
  credit: DreamFactory-Development
  creditlink: http://tat306.github.io/DreamFactory/development
---

<ul class="post-list">
{% for post in site.categories.development %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
