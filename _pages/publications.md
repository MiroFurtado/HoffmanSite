---
title: "Hoffman Lab - Publications"
layout: gridlay
excerpt: "Hoffman Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications



## Highlights

<div class="container" style="position: relative; right: 2%">


{% for highlight in site.data.highlights %}

<div class="row">
<div class="col-sm-8">
<div class="well">
<img style="{{highlight.style}}" src="{{ site.url }}{{ site.baseurl }}/images/highlights/{{highlight.image}}"/>
<h3 style="text-align: center">{{highlight.title}}</h3>
<em>{{highlight.description}}</em>
<br/>
<a style="float:right" class="nounder" href="{{highlight.url}}">{{highlight.publication}}</a>
</div>
</div>
</div>

{% endfor %}
</div>

## All

<br/>

{% for article in site.data.pubs %}

<h4><a href="{{ article.url }}">{{ article.title }}</a></h4>
<dd>
<div style="margin-left: 40px;">
<i>{{ article.authors }}</i><br/>
{{ article.cite }}
</div>

{% endfor %}

<br/><br/>
