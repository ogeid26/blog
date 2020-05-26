---
layout: page
title: Books
permalink: /books.html
---

<p>
Book recommendations/reviews/thoughts.
</p>

You can check my book list over [here](https://www.notion.so/agendadiego/books-e94b8925165249638aba8d53690e9c39).

Do you disagree with some idea i have? Please feel free to send me a mail/make a comment on my book list! I'd love to argue the reasoning behind what i write :~)
<h2> Book Reviews </h2>

<ul>
	{% for post in site.posts %}
    {% if post.category contains "book", post.subcategory contains "review" %}
<li>

<h3><a href="{{ site.url }}{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>
</li>
{% comment %} <p>{{ post.excerpt }}</p> {% endcomment %}
{% endif %}
{% endfor %}
</ul>
