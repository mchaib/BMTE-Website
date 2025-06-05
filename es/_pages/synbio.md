---
title: "BMTE - Semillero de investigación"
layout: gridlay2
excerpt: "BMTE -- Research"
sitemap: false
tags: [10001, 10002,10003, 10004, 10005, 10006]
permalink: /es/synbio/
lang: es
---

<div class="text-center">
<img style="position:relative; left:0px" src="{{ site.url }}{{ site.baseurl }}/images/logopic/group_incubator.png" height="200" width="auto" class="rounded float-right">
</div>

# Semillero de Investigación: Nuestra Historia
El semillero de investigación de Biología Sintética fue inscrito el 19 de agosto de 2022 por Clara Isabel Bermúdez Santanda, Profesora Asociada del Departamento de Biología como una iniciativa inter-institucional que constituye un espacio colaborativo en el que estudiantes de diferentes disciplinas cuentan con el apoyo de profesores, interesados en el desarrollo de la biología sintética en la Universidad Nacional sede Bogotá

## Misión
En el semillero de investigación estamos motivados por la convicción de que las asociaciones heterospecíficas (simbiosis) desafían nuestra concepción de la individualidad biológica y que la comprensión de los mecanismos moleculares que los subyacen tiene fuertes implicaciones para la innovación evolutiva y las aplicaciones en diversas industrias.

## Visión
Dentro de cinco años, el semillero pretende ser capaz de realizar experimentos computacionales en modelos evolutivos que pueden representar conversiones de información y las ganancias de energía resultantes utilizables por entidades en evolución. Esto se puede lograr tanto a nivel de organismos virtuales como de proteínas naturales y ARN.


### Lineas de investigación
Actualmente tenemos 4 lineas de investigación, las cuales son las siguientes:

<div class="container">
<div class="row">
<div class="col-7">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/group_incubator.png" class="img-responsive" width="20%" style="float: left"/>
</div>
<div class="col-8 col-md-6">
<br>


1. Análisis de la relación estructura-función en biología molecular desde la perspectiva de la continuidad organizacional a niveles jerárquicos

2. Evolución de regiones genómicas no codificantes

3. Identificación de los mecanismos moleculares subyacentes a las interacciones simbióticas 

4. Diseño computacional de circuitos genéticos en microorganismos para modular la fisiología del huésped

</div>
</div>
</div>
### Proyectos en curso de SynBio
{% for project in site.data.project %}

{% if project.ongoing == 0 %}
<div class="row">
<div class="well">

#### {{ project.title }} ({{ project.key}})

**Researchers:** {{project.researchers}}

<a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#31f51f; hover:#1ff54f;" role="button" aria-expanded="false">**Summary**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
{{ project.summary }}
</div></div>
</div>
</div>
<br/>

{% endif %}

{% endfor %}


<p> &nbsp; </p>

#### ... Y más
