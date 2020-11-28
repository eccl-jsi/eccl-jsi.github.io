---
title: "ECCL - Publications"
layout: gridlay
excerpt: "ECCL - Publications"
sitemap: false
permalink: /publications/
---


# Publications

Publications authored and co-authored by current team members

## Highlights

(For a [Full List](#full-list) and [Popular Science Articles](#popular-science-articles) in Slovene see below)

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-success">{{ publi.news1 }}</p>
  <p> {{ publi.news2 }}</p>
  <div class="clearfix"></div>
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


## Full List

{% for publi in site.data.publist %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" style="float: left;" width="120" height="100">
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <p class="text-success">{{ publi.news1 }}</p>
  <div class="clearfix"></div>
  <hr>
{% endfor %}

<hr>
<p> &nbsp; </p>

## Popular Science Articles

{% for publi in site.data.poppublist %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" style="float: left;" width="120" height="100">
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <p class="text-success">{{ publi.news1 }}</p>
  <div class="clearfix"></div>
  <hr>
{% endfor %}

