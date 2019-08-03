---
title: "Team"
layout: gridlay
excerpt: "Team members"
sitemap: false
permalink: /team/
---
# LAB LEADER
{% assign number_printed = 0 %}
{% for member in site.data.members_pi %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix" >
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: middle;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}><br>
  <h6>
    {{ member.linkedin }} | 
    {{ member.googlescholar }} | 
    {{ member.researchgate }} | 
    {{ member.twitter }}| 
    {{ member.orcid }}
  </h6><br>
  {{ member.biography }}

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## GROUP LEAD

{% assign number_printed = 0 %}
{% for member in site.data.members_lead %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}> 
  <h6>{{ member.linkedin }} | {{ member.googlescholar }} | {{ member.researchgate }} | {{ member.twitter }} | {{ member.orcid }}</h6>

  <div id="{{ member.modalid }}" class="modal">
   {{ member.research }}
   {{ member.biography }}
   <a href="#" rel="modal:close">Close</a>
  </div>
  <p><a href="#{{ member.modalid }}" rel="modal:open">Career Biography</a></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


##  PhD STUDENTS
{% assign number_printed = 0 %}
{% for member in site.data.members_phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}> 
  <h6>{{ member.linkedin }} | {{ member.googlescholar }} | {{ member.researchgate }} | {{ member.twitter }} | {{ member.orcid }}</h6>

  <div id="{{ member.modalid }}" class="modal">
   {{ member.research }}
   {{ member.biography }}
   <a href="#" rel="modal:close">Close</a>
  </div>
  <p><a href="#{{ member.modalid }}" rel="modal:open">Career Biography</a></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## MPhil Students
{% assign number_printed = 0 %}
{% for member in site.data.members_mphil %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}> 
  <h6>{{ member.linkedin }} | {{ member.googlescholar }} | {{ member.researchgate }} | {{ member.twitter }} | {{ member.orcid }}</h6>

  <div id="{{ member.modalid }}" class="modal">
   {{ member.research }}
   {{ member.biography }}
   <a href="#" rel="modal:close">Close</a>
  </div>
  <p><a href="#{{ member.modalid }}" rel="modal:open">Career Biography</a></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## BSc Students
{% assign number_printed = 0 %}
{% for member in site.data.members_bsc %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}> 
  <h6>{{ member.linkedin }} | {{ member.googlescholar }} | {{ member.researchgate }} | {{ member.twitter }} | {{ member.orcid }}</h6>

  <div id="{{ member.modalid }}" class="modal">
   {{ member.research }}
   {{ member.biography }}
   <a href="#" rel="modal:close">Close</a>
  </div>
  <p><a href="#{{ member.modalid }}" rel="modal:open">Career Biography</a></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.members_alumini %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><{{ member.email }}> 
  <h6>{{ member.linkedin }} | {{ member.googlescholar }} | {{ member.researchgate }} | {{ member.twitter }} | {{ member.orcid }}</h6>

  <div id="{{ member.modalid }}" class="modal">
   {{ member.research }}
   {{ member.biography }}
   <a href="#" rel="modal:close">Close</a>
  </div>
  <p><a href="#{{ member.modalid }}" rel="modal:open">Career Biography</a></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

