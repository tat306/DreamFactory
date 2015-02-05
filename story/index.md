---
layout: page
title: story
excerpt: "Schedule for this project."
search_omit: true
image:
  feature: p_st_index_feature.png
  credit: DreamFactory-Story
  creditlink: http://tat306.github.io/DreamFactory/story
---

<ul class="post-list">
{% for post in site.categories.story %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
