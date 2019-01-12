---
title: "Hoffman Lab - News"
layout: gridlay
excerpt: "Hoffman Lab -- News"
sitemap: false
permalink: /news/
---

# News


<div class="container" style="position: relative; right: 2%">


{% for newsitem in site.data.news %}

<div class="row">
<div class="col-sm-8">
<div class="well">
{% if newsitem.image %}<img style="{{newsitem.style}}" src="{{ site.url }}{{ site.baseurl }}/images/news/{{newsitem.image}}"/>{% endif %}
<h3 style="text-align: center" data-toc-text="{{newsitem.toc}}">{{newsitem.title}}</h3>
<em>{{newsitem.description}}{% if newsitem.url %}<a class="nounder" href="{{newsitem.url}}">...read more</a>{% endif %}</em><br/>
{% if newsitem.type %}<i style="float:right;" class="material-icons">{{newsitem.type}}</i>
{% else %} <i style="float:right" class="material-icons">info</i>
{% endif %}

</div>
</div>
</div>

{% endfor %}
</div>