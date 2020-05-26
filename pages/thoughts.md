---
title: Thoughts
layout: page
permalink: /thoughts.html
---

<h2> Articles </h2>
<ul>
{% assign sorted-posts = site.posts | sort: 'date' %}
{% for post in sorted-posts %}
{% if post.category contains "article" %}
<li>
<h3> <a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>	
</li>
{% endif %}
{% endfor %}
</ul>


<h2> Poems </h2>
<ul>
{% assign sorted-posts = site.posts | sort: 'date' %}
{% for post in sorted-posts %}
{% if post.category contains "poem" %}
<li>
<h3> <a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>	
</li>
{% endif %}
{% endfor %}
</ul>
