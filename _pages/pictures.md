---
title: "ECCL - Pictures"
layout: piclay
excerpt: "ECCL - Pictures"
permalink: /pictures/
---

# Pictures
Jump to: [JSI](#JSI), [Outreach](#Outreach)

(Page under construction…)


## JSI

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
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

Our fluorine vacuum line
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/gallery/Lab.jpg" width="60%" >
</figure>

Single-Crystal X-ray Diffractometer 
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/gallery/Gemini.gif" width="60%" >
</figure>

## Outreach
Liquid Nitrogen Geysir - from the [Festival della Scienza](http://festival2019.festivalscienza.it/site/home/programma-2019/esperimenti-chimici-in-cucina.html) 2019, Genoa, Italy.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/gallery/IMG_2218.jpg" width="60%">
</figure>
