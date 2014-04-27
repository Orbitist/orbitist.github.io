---
layout: page
title: Home
---
##List of content here:
<hr>
{% for post in site.posts limit: 10 %}
{% if post.listed %}
###[{{ post.title }}]({{ post.url }})
<p class="lead">{{ post.description }}</p>
<hr>
{% endif %}
{% endfor %}