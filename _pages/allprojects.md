---
title: "Projects"
layout: textlay
excerpt: "BMTE - Ongoing and Past Projects"
sitemap: false
permalink: /allprojects.html
---

# Ongoing Projects

### BMTE (Theoretical and Evolutionary Molecular Biology)
{% for project in site.data.project %}
{% if project.ongoing == 1 %}
<div class="row">
<div class="well">

##### {{ project.key }}
<br>
#### {{ project.title }}
<br>

**Researchers:** {{project.researchers}}

<a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#31f51f; hover:#1ff54f;" role="button" aria-expanded="false">**Summary**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
<br>
{{ project.summary }}
</div></div>
</div>
</div>
{% endif %}
{% endfor %}

### SynBio Ongoing projects
{% for project in site.data.project %}

{% if project.ongoing == 0 %}
<div class="row">
<div class="well">

##### {{ project.key }}
<br>
#### {{ project.title }}
**Researchers:** {{project.researchers}}
<br>
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

#### ... and so much more.
