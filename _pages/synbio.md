---
title: "BMTE - Research Incubator"
layout: gridlay2
excerpt: "BMTE -- Research"
sitemap: false
tags: [10001, 10002,10003, 10004, 10005, 10006]
permalink: /synbio/
---

<div class="text-center">
<img style="position:relative; left:0px" src="../images/logopic/group_incubator.png" height="200" width="auto" class="rounded float-right">
</div>

# BMTE Research Incubator: Our History
The Synthetic Biology Research center was registered on August 19, 2022 by Clara Isabel Bermúdez Santanda, Associate Professor of the Department of Biology as an inter-site initiative that constitutes a collaborative space in which students from different disciplines have support from professors, interested in the development of synthetic biology at the Universidad Nacional.

## Mission
In the theoretical and evolutionary molecular biology research group (BMTE), we are motivated by the conviction that heterospecific associations (symbiosis) challenge our conception of biological individuality and that understanding the molecular mechanisms that underlie them has strong implications for evolutionary innovation and applications in various industries.
## Vision
Within five years, the Group aims to be able to conduct computational experiments on evolutionary models that can represent information conversions and the resulting energy gains usable by evolving entities. This can be achieved at the level of both virtual organisms and natural proteins and RNA.

### Lines of Research
We currently have 4 lines of research, which are as it follows:

<div class="container">
<div class="row">
<div class="col-7">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/group_incubator.png" class="img-responsive" width="20%" style="float: left"/>
</div>
<div class="col-8 col-md-6">
<br>


1. Analysis of the structure-function relationship in molecular biology from the perspective of organizational continuity at hierarchical levels

2. Evolution of non-coding genomic regions

3. Identification of molecular mechanisms underlying symbiotic interactions

4. Computational design of genetic circuits in microorganisms to modulate host physiology

</div>
</div>
</div>
### SynBio Ongoing projects
{% for project in site.data.project %}

{% if project.ongoing == 0 %}
<div class="row">
<div class="well">

#### {{ project.title }}
##### {{ project.key }}
**Researchers:** {{project.researchers}}

<a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#31f51f; hover:#1ff54f;" role="button" aria-expanded="false">**Summary**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
<br>
{{ project.summary }}
</div></div>
</div>
</div>
<br/>

{% endif %}

{% endfor %}

<p> &nbsp; </p>

#### ... and more.
