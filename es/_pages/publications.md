---
title: "BMTE - Publications"
layout: gridlay
excerpt: "BMTE research Group -- Publications."
sitemap: false
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009]
permalink: /es/publications/
lang: es
---

# Publicaciones
### Publicaciones destacadas
(Para ver la lista completa de publicaciones, da click [aqui](#lista-de-publicaciones)


{% assign number_printed = 0 %}
{% for publi in site.data.research_themes %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/publications/{{ publi.image }}" class="img-responsive" width="40%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
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

<p> &nbsp; </p>


## Lista de publicaciones

### Grupo de Investigación (BMTE)
<div class="publications">
{% bibliography -f mbte_publications -q @*[published={{1}}]* %}

</div>
