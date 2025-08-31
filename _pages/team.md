---
title: "Team"
layout: gridlay
sitemap: false
permalink: /team/
---

### Team





<div class="jumbotron">
{% for member in site.data.pi %}
<div class="row">
<div class="col-sm-2">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-9 col-xs-12">
<h5>{{ member.name }} (胡国标)</h5>
<i>{{ member.info }}</i><br>
Assistant Professor, IoT Thrust, Information Hub
</div>
</div>
{% endfor %}

<div class="row">
<div class="col-sm-2">
<img src="{{ site.url }}{{ site.baseurl }}/images/shiyi.jpg" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-9 col-xs-12">
<h5>Shiyi (十一)</h5>
<i>Team Mascot</i>
</div>
</div>

</div>


### Current Students

<div class='jumbotron'>
{% for member in site.data.team_members %}
<div class="row">
<div class="col-sm-2">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-10 col-xs-12">
<h5>{{ member.name }}</h5>
<i>{{ member.info }}<br></i>
Email: <i>{{ member.email }}<br></i>
Graduated from: <i>{{ member.graduated }}</i><br>
Publications: {% assign publications = member.publications | split: ", " %}
{% for pub in publications %}[{{ pub }}]{% if forloop.last == false %} {% endif %}{% endfor %}<br>
</div>
</div>
{% endfor %}
</div>

### Visiting Members

<div class='jumbotron'>
{% for member in site.data.visiting_student %}
<div class="row">
<div class="col-sm-2">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-10 col-xs-12">
<h5>{{ member.name }}</h5>
<i>{{ member.info }}<br></i>
<i>{{ member.duration }}<br></i>
Publications: {% assign publications = member.publications | split: ", " %}
{% for pub in publications %}[{{ pub }}]{% if forloop.last == false %} {% endif %}{% endfor %}<br>
</div>
</div>
{% endfor %}
</div>

### Alumni

<div class='jumbotron'>
{% for member in site.data.alumni %}
<div class="row">
<div class="col-sm-2">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-10 col-xs-12">
<h5>{{ member.name }}</h5>
<i>{{ member.position }}<br></i>
<i>{{ member.info }}<br></i>

Publications: {% assign publications = member.publications | split: ", " %}
{% for pub in publications %}[{{ pub }}]{% if forloop.last == false %} {% endif %}{% endfor %}<br>
</div>
</div>
{% endfor %}
</div>

