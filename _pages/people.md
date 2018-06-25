---
title: "Hoffman Lab - People"
layout: gridlay
excerpt: "Hoffman Lab: People"
sitemap: false
permalink: /people/
---

# Group Members

<div class="row">

<div class="col-sm-6 clearfix">
## Professor 
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/JennyHoffman_large.jpg" class="img-responsive" width="25%" style="float: left" />
  <h4>Jenny Hoffman</h4>
  <i><jhoffman@physics.harvard.edu><br>CV: <a href="http://users.physics.harvard.edu/~jhoffman/HoffmanCVshort.pdf">Short</a>, <a href="http://users.physics.harvard.edu/~jhoffman/HoffmanCVlong.pdf">Extended</a><br><a href="http://users.physics.harvard.edu/~jhoffman/HoffmanCVshort.pdf">Personal website</a></i>
</div>

<div class="col-sm-6 clearfix">
## Research Associate
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/Jason.jpg" class="img-responsive" width="25%" style="float: left" />
  <h4>Jason Hoffman</h4>
  <i><jasonhoffman@fas.harvard.edu></i>
</div>
</div>

## Post-docs

{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i><{{ member.email}}></i>
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




## Grad Students 
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i><{{ member.email }}></i>
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

## Undergraduates
{% assign number_printed = 0 %}
{% for member in site.data.undergrads %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i><{{ member.email }}></i>
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
