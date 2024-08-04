---
title: "News"
layout: textlay
sitemap: false
permalink: //all news/
---

## News

<div class="jumbotron">
{% for article in site.data.news %}
<b>{{ article.date }}</b>

{{ article.headline }}
{% endfor %}

</div>
