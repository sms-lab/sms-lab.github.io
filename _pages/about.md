---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---

<!--循环遍历 site.data.pi 数据，该数据定义了项目的主要参与者或成员 -->
{% for member in site.data.pi %}

<div class="jumbotron">
<div class="row">
<div class="col-sm-4 text-center">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" style="width:100%; max-width:180px"/>
<div class="icon-container">
{% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-2x"></i></a> {% endif %}
{% if member.scholar %}<a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square fa-2x"></i></a> {% endif %}
{% if member.researchgate %}<a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square fa-2x"></i></a> {% endif %}
{% if member.cv %}<a href="{{ site.url }}{{ site.baseurl }}/{{ member.cv }}" target="_blank"><i class="ai ai-cv-square fa-2x"></i></a> {% endif %}
{% if member.github %}<a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-2x"></i></a> {% endif %}
</div>
</div>
<div class="col-sm-8 col-xs-12">
<h4>{{ member.name }}</h4>
<h4><i>{{ member.info }}</i></h4>
<ul style="overflow: hidden; padding-left: 0">
Dr. Hu has published more than 100 peer-reviewed technical papers in prestigious journals and international conferences, with 5 being ESI highly cited papers. He was a recipient of the Best Paper Finalist Award at the SPIE Conference on Smart Structures/NDE in 2018. He has filed 4 patents, including 1 Singapore patent and 3 Chinese patents. According to Google Scholar statistics in August 2024, his publications have received over 2900 citations with an H-index of 30. He is featured in the world's top 2% of Scientists List (2022) identified by Stanford University. He serves as reviewer for more than 60 SCI journals and guest editor for the Journal of Physics D: Applied Physics and ASCE Journal of Environmental Engineering.
</ul>
</div>
</div>
</div>
{% endfor %}

<div class="jumbotron">
  <h4>Research Interests</h4>
  <ul>
    <li>Energy Harvesting</li>
    <li>Acoustic-Elastic Metamaterials</li>
    <li>Nonlinear Dynamics</li>
    <li>Piezoelectric Materials</li>
  </ul>
</div>

<div class="jumbotron">
  <h4>Appointments</h4>
  <ul>
    <li>2022.11-Present, Assistant Professor, The Hong Kong University of Science and Technology (GZ)</li>
    <li>2020.03-2022.10, Research Fellow, Nanyang Technological University</li>
    <li>2019.08-2019.12, Research Associate, The University of Auckland</li>
  </ul>
</div>

<div class="jumbotron">
  <h4>Education</h4>
  <ul>
    <li>2015.08-2019.07, Ph.D. in Mechanical Engineering, The University of Auckland</li>
    <li>2012.09-2015.07, M.Sc in Mechanical Engineering, Southwest Jiaotong University</li>
    <li>2010.09-2012.07, Diplôme d'Ingénieur in General Engineering, École centrale de Paris</li>
    <li>2008.09-2012.07, B.Ec. in Mechanical Engineering, Southwest Jiaotong University</li>
  </ul>
</div>

<div class="jumbotron">
  <h4>Honors & Awards</h4>
  <ul>
    <li>2019.05, Research Excellence Scholarship, Department of Mechanical Engineering, UoA, New Zealand</li>
    <li>2018.11, Merit Scholarship, Department of Mechanical Engineering, UoA, New Zealand</li>
    <li>2016.07, CSC Doctoral Scholarship, China Scholarship Council, China</li>
    <li>2015.05, EET PhD Research Scholarship, Energy Education Trust, New Zealand</li>
    <li>2014.09, First-class Postgraduate Scholarship, SWJTU, China</li>
    <li>2013.09, First-class Postgraduate Scholarship, SWJTU, China</li>
    <li>2012.09, First-class Postgraduate Scholarship, SWJTU, China</li>
    <li>2010.07, Eiffel Scholarship, Ministry of Foreign Affairs and International Development, France</li>
    <li>2010.05, First-class Undergraduate Scholarship, SWJTU, China</li>
    <li>2009.11, National Scholarship, Ministry of Education, China</li>
    <li>2009.11, Merit Student, SWJTU, China</li>
    <li>2009.05, First-class Undergraduate Scholarship, SWJTU, China</li>
  </ul>
</div>

{% if site.data.people %}

<div class="jumbotron">
  <h4>Students and Mentoring</h4>
  <ul>
    {% for student in site.data.people %}
      <li>{{ student.name }}, {{ student.location }} ({{ student.degree }}, {{ student.year }})</li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<!--
<div class="jumbotron">
  <h4>Collaborators</h4>
  <div style='display:flex; justify-content:center; flex-wrap:wrap;'>
    {% for collaborator in site.data.collaborators %}
    <div style='display: inline-block; margin: 10px; text-align: center;'>
    <a href="{{ collaborator.url }}" target="_blank">
    <img src='{{ site.url }}{{ site.baseurl }}/images/{{ collaborator.image }}' style='max-height: 120px; max-width: 200px;'/><br>
    <span>{{ collaborator.name }}</span><br>
    <span>PI: {{ collaborator.PI }}</span>
    </a>
    </div>
    {% endfor %}
  </div>
</div>
--> 


