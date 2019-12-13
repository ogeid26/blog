---
layout: default
permalink: /music.html
---
# Music

Here you'll find my reviews on bands and artists.

## Reviews
<ul>
	{% for post in site.posts %}
    {% if post.category contains "music" %}
<li>
<a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a>	
</li>
<p>{{ post.excerpt }}</p>
        {% endif %}
        {% endfor %}
</ul>
