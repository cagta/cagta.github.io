---
title: bookmarks
layout: page
permalink: /bookmarks
nav: custom
custom-nav: 
    - '<a href="/about" title="about">about</a>'
---

<div class="callout" markdown="1">

## What are bookmarks?

This is what I like from the internet. The best way to follow is via [the RSS feed](/rss).

</div>


{% for post in site.categories.bookmarks %}
<section class="bookmarks-entry" markdown="1">
<h1><a href="{{post.url}}" style="text-decoration: none;">{{post.title}}</a></h1>

{{post.content}}

<p class="bookmarks-date-line"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%B %d, %Y" | downcase}}</time></p>
</section>


{% endfor %}

