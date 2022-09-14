---
title: "ML4SCI@BC - Team"
layout: gridlay
excerpt: "ML4SCI@BC: Team members"
sitemap: false
permalink: /team/
---
# PIs

{% assign number_printed = 0 %}
{% assign number_per_row = 3 %}
{% assign number_last = number_per_row | minus: 1 %}

{% for member in site.data.team_pi %}

{% assign new_row = number_printed | modulo: number_per_row %}
{% if new_row == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.website }}">{{ member.name }}</a></h4>
  <i>{{ member.info }} </i>
  <br> {{ member.department }}
  <br> <{{ member.email }}>
  <ul style="overflow: hidden">
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if new_row == number_last %}
</div>
{% endif %}

{% endfor %}

{% assign new_row = number_printed | modulo: number_per_row %}
{% if new_row != 0 %}
</div>
{% endif %}

<br/>
## Affliated PIs
{% assign number_printed = 0 %}
{% for member in site.data.team_affiliate %}

{% assign new_row = number_printed | modulo: number_per_row %}

{% if new_row == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.website }}">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i> 
  <br> {{ member.department }}
  <br> <{{ member.email }}>
  <ul style="overflow: hidden">
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if new_row == number_last %}
</div>
{% endif %}

{% endfor %}

{% assign new_row = number_printed | modulo: number_per_row %}
{% if new_row != 0 %}
</div>
{% endif %}

<br/>
## Team Members
{% assign number_printed = 0 %}
{% for member in site.data.team_current %}
{% assign new_row = number_printed | modulo: number_per_row %}

{% if new_row == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i> 
  <br> {{ member.department }}
  <br> <{{ member.email }}>
  <ul style="overflow: hidden">
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if new_row == number_last %}
</div>
{% endif %}

{% endfor %}

{% assign new_row = number_printed | modulo: number_per_row %}
{% if new_row != 0 %}
</div>
{% endif %}

<br/>
## Student Group
<a href="https://mig-site.vercel.app/">Machine Inelligence Group (MIG)</a>
<div class="row">
</div>
<br/>
## Support
<div class="row">
<a href="mailto:mary.mulkeen@bc.edu">Mary Mulkeen</a> is helping us with administration.
</div>
