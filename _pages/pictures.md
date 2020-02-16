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

Photochemical synthesis of KrF<sub>2</sub> from liquid F<sub>2</sub> and solid Kr at −196 °C (Photo: M. Lozinšek)
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/KrF2-Photosynthesis-C.jpg" width="40%" >
</figure>
This image was published in:
- <i>Nature Chemistry</i>
<br>In Your Element: [The world of krypton revisited](https://www.nature.com/articles/nchem.2538) 
<br>Matic Lozinšek and Gary J. Schrobilgen consider krypton — namesake of Superman's home planet — its superoxidant compounds, and their roles in coaxing elements into their highest oxidation states
- <i>ACS Central Science</i>
<br>[Coaxing Reactivity from the Noble Gases](https://pubs.acs.org/doi/10.1021/acscentsci.9b00631) by Bethany Halford
<br>Rule-breaking chemists go to extremes to make the least-reactive elements forge bonds
- <i>Chemical & Engineering News</i>
<br>[To get noble gases to forge bonds, chemists go to extremes](https://cen.acs.org/materials/inorganic-chemistry/IYPT-get-noble-gases-to-forge-bonds-chemists-go-to-extremes/97/i22) by Bethany Halford
<br>Despite challenging conditions and a lack of funding, some researchers still see rewards in coaxing reactivity from these nearly inert elements 

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
