---
title: "Clark Lab - Team"
layout: gridlay
excerpt: "Clark Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [current lab members](#team), [lab alumni](#lab alumni), [undergraduate alumni](#undergraduate alumni).

## Team
{% for member in site.data.team_members %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br>{{ member.info }}
  <br>contact: <{{ member.email }}></i>
</div>

{% endfor %}


## Lab Alumni

{% for member in site.data.alumni_members %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="12.5%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br>{{ member.info }}
  <br>{{ member.next_destination }}
</div>

{% endfor %}


## Undergraduate Alumni

{% for member in site.data.alumni_undergraduates %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="12.5%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br>{{ member.next_destination }}
</div>

{% endfor %}
