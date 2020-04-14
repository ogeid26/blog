---
title: Thoughts
layout: page
permalink: /thoughts.html
---

<ul>
{% assign sorted-posts = site.posts | sort: 'date' %}
{% for post in sorted-posts %}
{% if post.category contains "thoughts" %}
<li>
<h2> <a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h2>	
</li>
{% endif %}
{% endfor %}
</ul>

