---
title: "News"
layout: textlay
excerpt: "I-Machine-Think in the ILLC"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
