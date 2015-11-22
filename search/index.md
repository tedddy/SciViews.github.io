---
layout: page
title: "Search"
date: 
modified:
excerpt:
image:
  feature:
search_omit: true
sitemap: false
---
  
<!-- Search form -->
<form method="get" action="{{ site.url }}/search/" data-search-form
class="simple-search">
  <label for="q">Search {{ site.title }} titles for:</label>
  <input type="search" name="q" id="q" placeholder="What are you looking for?"
    data-search-input id="goog-wm-qt" autofocus />
  <input type="submit" value="Search Titles" id="goog-wm-sb" />
</form>

<!-- Search results placeholder -->
<h6 data-search-found>
  <span data-search-found-count></span> result(s) found for &ldquo;<span
    data-search-found-term></span>&rdquo;.
</h6>
<ul class="post-list" data-search-results></ul>

<!-- Search result template -->
<script type="text/x-template" id="search-result">
  <li><article>
    <a href="##Url##"><b>##Title##</b> <span class="excerpt">##Excerpt##</span></a>
  </article></li>
</script>

<!-- Search with Google or look at tags -->
<div class="simple-search">
  <script type="text/javascript">
    var GOOG_FIXURL_LANG = 'en';
    var GOOG_FIXURL_SITE = '{{ site.url }}'
  </script>
  <script type="text/javascript"
    src="//linkhelp.clients.google.com/tbproxy/lh/wm/fixurl.js">
  </script>
</div>

<div class="simple-search">
  Or look in the
  <b><a href="../tags/" target="_self">tags</a></b>
  in the whole site.
</div>