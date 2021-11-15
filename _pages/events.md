---
title: "ML4SCI@BC - Events"
layout: gridlay
excerpt: "ML4SCI@BC: Events"
sitemap: false
permalink: /events/
---
# Events

{% assign number_printed = 0 %}
{% assign number_per_row = 3 %}
{% assign number_last = number_per_row | minus: 1 %}
<div class="row">
{% for event in site.data.events %}

<div class="col-sm-10 clearfix">
  <table border=0>
  <tr>
  <td><img src="{{ site.url }}{{ site.baseurl }}/images/{{ event.photo }}"  height="150px" style="float: left" />
  </td>
  <td>
  <h4>{{ event.title }}</h4>
  <b>Speaker:</b> <a href="{{ event.website }}">{{ event.speaker }}</a>
  <br/> <b>Time:</b> {{ event.time }}
  <br/> <b>Location:</b> {{ event.location }}
  <br/><br/> <b>Description:</b> <i>{{ event.description }} </i>
  </td>
  </tr>
  </table>
</div>

{% endfor %}
</div>
