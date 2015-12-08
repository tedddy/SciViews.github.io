---
layout: page
title: Recipes
excerpt: "SciViews recipes sorted by date."
search_omit: true
---

<div class="simple-search">
  You may also look for items by <b><a href="../tags/" target="_self">tags</a></b>.
</div>

<ul class="post-list">
{% for post in site.categories.recipes %} 
  {% if post.categories[0] == "recipes" %}
  <li><article><a href="{{ site.url }}{{ post.url }}"><b>{{ post.title }}</b> <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
  {% endif %}
{% endfor %}
</ul>
