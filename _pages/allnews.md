---
title: "News"
layout: textlay
excerpt: "I-Machine-Think in the ILLC"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p><b>{{ article.date }}</b><br>
{% if article.content %}
{{ article.content }}
{% else %}
{{ article.headline }}
{% endif %}
<br>
{% if article.image %} <img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image }}" width='70%' style='float: centre'/> {% endif %}
<br>
</p>

{% endfor %}
