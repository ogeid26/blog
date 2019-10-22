---
layout: default
permalink: /music.html
---
# Music

Here you'll find my reviews on bands and artists.

## Reviews
<ul>
	{% for post in site.posts | where "category", "music and "subcategory", "review"" %}
<li>
<a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a>	
</li>
<p>{{ post.excerpt }}</p>
{% endfor %}
</ul>
