---
layout: page
title: Programming
permalink: /programming.html
---

Interesting stuff on programming (particularly on personal projects and uni stuff)
<ul>
	{% for post in site.posts %}
    {% if post.category contains "programming" %}
<li>
<h3><a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>
</li>
{% comment %} <p>{{ post.excerpt }}</p> {% endcomment %}
{% endif %}
{% endfor %}
</ul>
