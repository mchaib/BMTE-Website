---
title: "Projects"
layout: textlay
excerpt: "BMTE - Ongoing and Past Projects"
sitemap: false
permalink: /es/allprojects.html
lang: es
---

# Proyectos en Curso

### BMTE (Biología Molecular Teórica y Evolutiva)
{% for project in site.data.project %}
{% if project.ongoing == 1 %}
<div class="row">
<div class="well">

##### {{ project.key}}
<br>
#### {{ project.title }}
<br>

**Investigadores:** {{project.researchers}}

<a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#31f51f; hover:#1ff54f;" role="button" aria-expanded="false">**Resumen**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
<br>
{{ project.summary }}
</div></div>
</div>
</div>
{% endif %}
{% endfor %}

### Proyectos en curso en SynBio
{% for project in site.data.project %}
{% if project.ongoing == 0 %}
<div class="row">
<div class="well">

##### {{ project.key}}
<br>
#### {{ project.title }}
<br>

**Investigadores:** {{project.researchers}}

<a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#31f51f; hover:#1ff54f;" role="button" aria-expanded="false">**Resumen**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
<br>
{{ project.summary }}
</div></div>
</div>
</div>
{% endif %}
{% endfor %}


