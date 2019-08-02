---
title: "Team"
layout: gridlay
excerpt: "Team members"
sitemap: false
permalink: /team/
---
# LAB LEADER
{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix" >
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br>email: <{{ member.email }}><br>
  <h6>
    {{ member.linkedin }} | 
    {{ member.googlescholar }} | 
    {{ member.researchgate }} | 
    {{ member.twitter }}| 
    {{ member.orcid }}
  </h6>
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

## GROUP LEAD

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

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


##  STUDENTS
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="15%" style="float: left;" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
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

<!--
## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  </ul>
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


<table align="center" style="width:100%">
 <tr>
    <th>Visitors</th>
    <th>Master Students</th>
    <th>Bachelor Students</th>
  </tr>
  <tr>
    <td>Nikolaos Iliopoulos, Spring 2016</td>
    <td>Bert Visscher, Fall 2017</td>
    <td>Vishnu Saj, Spring 2017</td>
  </tr>
  <tr>
    <td>Vitaly Fedoseev, all of 2016</td>
    <td>Ahmad Jamalzada, Fall 2017</td>
    <td>Joey Braspenning, Spring 2017</td>
  </tr>
  <tr>
    <td>Ramakrishna Aluru, Summer 2018</td>
    <td>Tjerk Benschop, Summer 2017</td>
    <td>Margot Leemker, Spring 2017</td>
  </tr>
  <tr>
    <td>Changwei Zou, Spring 2018</td>
    <td>Oliver Ostojic, Spring 2016</td>
    <td>Sietske Lensen, Spring 2017</td>
  </tr>
  <tr>
    <td></td>
    <td>Farshaad Hoeseni, Fall 2015</td>
    <td>Alexander Vanstone, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Tjerk Benschop, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Arjo Andringa, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Daniëlle van Klink, Spring 2016</td>
  </tr>
</table>

## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration.
-->