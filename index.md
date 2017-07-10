---
layout: default
title: Home
description: Home of all things Viral Syndrome
image: /images/icon.social.png
---
{% for post in site.posts %}
<div class="article">
<div class="article_icon_area"><img class="article_icon" src="{{ post.wallpaper }}"></div>
<div class="article_data_area">
<a class="article_title" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
<br />
<span class="article_date">{{ post.date | date_to_string }}</span>
<hr />
<span class="article_summary">{{ post.summary }}</span>
</div>
</div>
<br />
{% endfor %}
