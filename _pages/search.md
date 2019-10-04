---
layout: page
title: Search
permalink: /search/
---

<div id="search-container">
    <div style="text-align: center">
        <h3>{{ site.data.search.en.header }}</h3>
        <input type="text" id="search-input" class="search-input" placeholder="Search"/>
    </div>
    <h3>{{ site.data.search.en.results }}</h3>    
    <ul id="results-container"></ul>
</div>

<script src="{{ site.baseurl }}/assets/simple-jekyll-search.min.js" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<div style="text-align: left !important;"><a href="{url}" title="{title}"><h1 style="text-align:left !important;">{title}</h1></a><span style="text-align:left !important;">{date}</span></div></a><span style="text-align:left !important;">{{site.data.common.flags.{{locale}}}}</span></div>',
    json: '{{ site.baseurl }}/search.json',
    noResultsText: 'No results found'
    });
</script>
