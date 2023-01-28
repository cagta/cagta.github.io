---
title: all of my updates
description: "all of my updates"
og-type: website
permalink: /blog/now
---

{% for post in site.categories.now %}
{% include blog-listing.html %}
{% endfor %}