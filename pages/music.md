---
layout: page
title: Music
permalink: /music.html
---


<p>
        Here you'll find my reviews on bands and artists.
</p>

<h1>Reviews</h1>
<ul>
{% assign sorted-posts = site.posts | sort: 'title' %}
{% for post in sorted-posts %}
{% if post.category contains "music" %}
<li>
<h2> <a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h2>	
</li>
{% endif %}
{% endfor %}
</ul>

