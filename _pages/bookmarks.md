---
title: bookmarks
layout: page
permalink: /bookmarks
---

<div class="callout" markdown="1">

## What are bookmarks?

things i like from here and there. the best way to follow is [the rss feed](/rss).

</div>


{% for post in site.categories.bookmarks %}
<section class="bookmarks-entry" markdown="1">
<h1><a href="{{post.url}}" style="text-decoration: none;">{{post.title}}</a></h1>

{{post.content}}

<p class="bookmarks-date-line"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%B %d, %Y" | downcase}}</time></p>
</section>


{% endfor %}

