---
title: "I-Machine-Think - Talks"
layout: gridlay
excerpt: "I-Machine-Think -- Talks."
sitemap: false
permalink: /talks/
---

## Talks

{% for publi in site.data.talks %}

  <b> <font size="+1"> {{publi.title }} </font></b> &nbsp; &#8226; &nbsp;
  <button onclick='window.open("{{ site.url }}{{ site.baseurl }}/documents/{{ publi.slides }}", "_blank")' style="float: right;"> slides </button>
  {{ publi.authors }} 
  <br/> <i> {{ publi.venue }} </i> &nbsp; &#8226; &nbsp;
  {{ publi.date }}, {{ publi.year }}

{% endfor %}

## Posters

{% for publi in site.data.posters %}

  <b> <font size="+1"> {{publi.title }} </font></b> &nbsp; &#8226; &nbsp;
  <button onclick='window.open("{{ site.url }}{{ site.baseurl }}/documents/{{ publi.poster }}", "_blank")' style="float: right;"> poster </button>
  {{ publi.authors }}
  <br/> <i> {{ publi.venue }} </i> &nbsp; &#8226; &nbsp;
  {{ publi.date }}, {{ publi.year }}

{% endfor %}

<br><br>
