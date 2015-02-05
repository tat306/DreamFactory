---
layout: page
title: timeline
excerpt: "Schedule for this project."
search_omit: true
image:
  feature: p_t_index_feature.png
  credit: DreamFactory-Timeline
  creditlink: http://tat306.github.io/DreamFactory/timeline
---

<ul class="post-list">
{% for post in site.categories.timeline %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
