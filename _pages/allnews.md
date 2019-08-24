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
{% if article.image3 %} 
<center>
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image }}" width='30%'/> 
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image2 }}" width='30%'/> 
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image3 }}" width='30%'/> 
</center>

{% elsif article.image2 %} 
<center>
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image }}" width='45%'/> 
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image2 }}" width='45%'/> 
</center>

{% elsif article.image %} 
<center>
<img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ article.image }}" width='60%'/> 
</center>

{% endif %}

<br>
</p>

{% endfor %}
