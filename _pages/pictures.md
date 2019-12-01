---
title: "ECCL - Pictures"
layout: piclay
excerpt: "ECCL -- Pictures"
permalink: /pictures/
---

# Pictures
Jump to: [JSI](#leiden), [1](#1), [2](#2), [3](#3)


## JSI

#### Photo 

#### Gallery
(Under construction)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

First advertisement.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageLeiden_red.jpg" width="60%" >
</figure>


## 1
From the [1](http://eccl.ijs.si).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageETH_red.jpg" width="60%">
</figure>

## 2
From the [2](http://eccl.ijs.si).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageCornell_red.jpg" width="60%">
</figure>

## 3
From the [3](http://eccl.ijs.si) ().
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageSTA_red.jpg" width="60%">
</figure>
