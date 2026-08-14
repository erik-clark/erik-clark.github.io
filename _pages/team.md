---
title: "Clark Lab - Team"
layout: gridlay
excerpt: "Clark Lab: Team members"
sitemap: false
permalink: /team/
---

<h1>Group Members</h1>

 **We are  looking for new PhD students, Postdocs, and Master's students to [join the team!]({{ site.url }}{{ site.baseurl }}/vacancies)**


Jump to [current lab members](#team), [lab alumni](#lab_alumni), or [former project students](#undergrad_alumni).

<h2 id="team">Team</h2>
{% for member in site.data.team_members %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="20%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br>{{ member.info }}
  <br>contact: <{{ member.email }}>
    {% if member.google_scholar %} [Google Scholar]({{ member.google_scholar}} ) {% endif %}
    {% if member.orcid %} [ORCiD]({{ member.orcid }}) {% endif %}
    {% if member.bluesky %} [BlueSky]({{ member.bluesky }}) {% endif %}
</div>

{% endfor %}
<br><br>


<h2 id="lab_alumni">Lab Alumni</h2>

{% for member in site.data.alumni_members %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="12.5%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br>{{ member.info }}
  <br><b>Next destination:</b> {{ member.next_destination }}
</div>

{% endfor %}
<br><br>


<h2 id="undergrad_alumni">Former Project Students</h2>

{% for member in site.data.alumni_undergraduates %}

<div class="row">
  <h4>{{ member.name }}</h4>
  <i>{{ member.role }}</i>
  <br><b>Next destination:</b> {{ member.next_destination }}
</div>

{% endfor %}
