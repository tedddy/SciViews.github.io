---
layout: page
title: Mastering SciViews and R
excerpt: "Guide for using R and SciViews."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.documentation %} 
  <li><article><a href="{{ site.url }}{{ post.url }}"><b>{{ post.title }}</b> <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
