---
title: "Hoffman Lab - People"
layout: gridlay
excerpt: "Hoffman Lab - People"
sitemap: false
permalink: /people/
---

# People

## Principal Investigator

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/hoffman3.png" class="img-responsive" width="20%" style="float: left" />
  <h3 data-toc-text="Principal Investigator">Jenny Hoffman </h3>
  <i>Professor<br>email:  <jhoffman@physics.harvard.edu></i>
  <ul style="list-style:none">  
  
  <li> Curriculum Vitae — <a href="http://physics.harvard.edu/~jhoffman/HoffmanCVshort.pdf">short</a>/<a href="http://physics.harvard.edu/~jhoffman/HoffmanCVlong.pdf">extended</a></li><br/>
  
 <li><a href="http://physics.harvard.edu/~jhoffman">Personal Website</a></li>
  
  </ul>
<br/><br/>
</div>

{% assign number_printed = 0 %}
{% for member in site.data.people %}


{% assign even_odd = number_printed | modulo: 2 %}

{% if member.header %}

{% if even_odd == 1 %}
</div>
{% endif %}

<h3>{{member.header}}</h3>

{% assign number_printed = 0 %}

{% else %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.photo %}<img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />{% endif %}
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <p>{{member.description}}
  </p>
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

