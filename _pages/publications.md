---
title: "Molecular Genetics and Cell Biology Group - Publications"
layout: gridlay
excerpt: "MGCBG -- Publications."
sitemap: false
permalink: /publications/
---


# Publications


{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well" style="background-color: #FFFFE0">
  <pubtit><a href="{{ publi.link.url }}">{{ publi.title }}</a></pubtit>
  <p><em><strong>{{ publi.authors }} {{ publi.date }}</strong></em></p> 
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="10%" style="float: left" />
  <p>{{ publi.description }}</p>
  
  <!-- <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p> -->
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


<!-- ## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
-->
