---
layout: default
permalink: /programming.html
---
# Programming

<ul>
	{% for post in site.posts %}
    {% if post.category contains "programming" %}
<li>
<a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a>	
</li>
<p>{{ post.excerpt }}</p>
{% endif %}
{% endfor %}
</ul>
