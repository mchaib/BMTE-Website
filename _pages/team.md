---
title: "BMTE members - Team"
layout: gridlay
excerpt: "Team members"
sitemap: false
permalink: /team/
---

<style>

.button {
    clear: none;
    border-radius: 8px;
    color: white;
    padding: 1px 20px;
    display: inline-block;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    cursor: pointer;
}

.linkedin {
    background-color: #1122FF;
    color: white;
    padding-top: 2px;
    border: 2px solid #0C090A;
}
.twitter {
    background-color: blue;
    color: white;
    padding-top: 3px;
    border: 2px solid #0C090A;
}
.orcid {
    text-align: center;
    text-decoration: none;
    font-size: 27px;
    background-color: #A6CE39;
    color: white;
    border: 2px solid #0C090A;
}
</style>

# Team Members

{% for member in site.data.team_members %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  
  <div style='margin-left:20%;'>
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}
  <br>email: {{ member.email }}</i>

  <p style="font-size:.8em">{{ member.short_bio }}</p>
</div>

<p style="clear:both;"></p>
<div class="row button-row" style="margin-left: 15%;">
{% if member.website1 %}
<div class="col-md-4">
<button
	class="button linkedin"
	onclick="window.location.href='{{ member.website1 }}'"
type="button"> <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16"> <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"/> </svg>
</button>
</div>
{% endif %}
{% if member.website2 %}
<div class="col-md-4">
<button
	class="button twitter"
	onclick="window.location.href='{{ member.website2 }}'"
type="button"> <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" class="bi bi-twitter" viewBox="0 0 16 16"> <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334q.002-.211-.006-.422A6.7 6.7 0 0 0 16 3.542a6.7 6.7 0 0 1-1.889.518 3.3 3.3 0 0 0 1.447-1.817 6.5 6.5 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.32 9.32 0 0 1-6.767-3.429 3.29 3.29 0 0 0 1.018 4.382A3.3 3.3 0 0 1 .64 6.575v.045a3.29 3.29 0 0 0 2.632 3.218 3.2 3.2 0 0 1-.865.115 3 3 0 0 1-.614-.057 3.28 3.28 0 0 0 3.067 2.277A6.6 6.6 0 0 1 .78 13.58a6 6 0 0 1-.78-.045A9.34 9.34 0 0 0 5.026 15"/> </svg>
</button>
</div>
{% endif %}
{% if member.website3 %}
<div class="col-md-4">
<button
	class="button orcid"
	onclick="window.location.href='{{ member.website3 }}'"
type="button"><strong> iD</strong></button>
</div>
{% endif %}
</div>


</div>
</div>
{% endfor %}

### Former visitors, BSc/MSc students
