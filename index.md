---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts %}

<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
=====================
{{ post.date | date_to_string }}
------------------
{{ post.content }}

{% endfor %}
