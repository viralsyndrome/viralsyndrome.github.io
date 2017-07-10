---
layout: default
title: Home
description: Home of all things Viral Syndrome
image: /images/icon.social.png
---
{% for article in site.articles %}
				<div class="article">
					<a class="article_title" href="{{ BASE_PATH }}{{ article.url }}">{{ article.title }}</a>
					<br />
					<span class="article_date">{{ article.date | date_to_string }}</span>
					<hr />
					<span class="article_summary">{{ article.summary }}</span>
				</div>
				<br />
{% endfor %}
