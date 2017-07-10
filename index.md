---
layout: default
title: Home
description: Home of all things Viral Syndrome
image: /images/icon.social.png
---
{% for post in site.posts %}
<div class="article">
<img class="article_icon" src="{{ post.wallpaper }}">
<a class="article_title" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
<span class="article_date">{{ post.date | date_to_string }}</span>
<hr />
<span class="article_summary">{{ post.summary }}</span>
</div>
<br />
{% endfor %}
