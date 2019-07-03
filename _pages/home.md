---
title: "I-Machine-Think - Home"
layout: homelay
excerpt: "I-Machine-Think at the ILLC"
sitemap: false
permalink: /
---

We are a research group at the University of Amsterdam

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
    </ol>

    {% assign slide_number = 0 %}

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
    {% for item in site.data.slider %}
        {% if item.first %} 
        <div class="item active">
        {% else %} 
        <div class="item">
        {% endif %}

        <img src="{{ site.url }}{{ site.baseurl }}/images/news/{{ item.image }}" height="40%" alt="Slide {{ slide_number }}" />
        <br>
        <p style="text-align:center;"> <i>{{ item.text }} </i> </p>
        <br>
        <br>

        </div>

        {% assign slide_number = slide_number | plus: 1 %}

    {% endfor %}
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
