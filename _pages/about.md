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
Dr. Guobiao Hu has published over 150 peer-reviewed journal and conference papers in leading venues, with multiple papers recognized as ESI Highly Cited Papers. His research contributions have been recognized by several international awards, including the ASME SMASIS Best Paper Award (2023) and the ASME SMASIS Ephrahim Garcia Best Paper Award (2024). He has filed several patents related to energy harvesting and intelligent sensing technologies. According to Google Scholar statistics, his publications have received over 4800 citations with an H-index of 37 (as of February 2026). Dr. Hu has been continuously listed among the World’s Top 2% Scientists (2022–2024) released by Stanford University. He serves as a reviewer for more than 60 SCI journals and has acted as a guest editor for journals including Journal of Physics D: Applied Physics.
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

<style>
#special-issues .editorial-list { list-style: none; padding: 0; margin: 0; }
#special-issues .editorial-list > li { display: flex; flex-wrap: wrap; align-items: center; gap: 12px 20px; padding: 15px 0; border-bottom: 1px solid #dce3eb; }
#special-issues .editorial-list > li:last-child { border-bottom: 0; padding-bottom: 0; }
#special-issues .editorial-details { flex: 1 1 280px; }
#special-issues .editorial-role { display: block; margin-top: 4px; color: #526174; font-size: 0.95rem; }
#special-issues .editorial-links { display: flex; flex-wrap: wrap; gap: 8px; }
#special-issues .special-issue-link { display: inline-flex; align-items: center; gap: 8px; padding: 8px 13px; border: 1px solid #0056b3; border-radius: 5px; background: #0056b3; color: #fff; font-weight: 600; font-size: 0.9rem; line-height: 1.4; text-decoration: none; }
#special-issues .special-issue-link:hover { background: #003d80; border-color: #003d80; color: #fff; text-decoration: underline; }
#special-issues .special-issue-link:focus-visible { outline: 3px solid #0056b3; outline-offset: 3px; }
</style>
<div class="jumbotron" id="special-issues">
  <h4>Guest Editorships &amp; Special Issues</h4>
  <ul class="editorial-list">
    <li>
      <div class="editorial-details"><strong>Journal of Physics D: Applied Physics</strong><span class="editorial-role">Guest Editor (2022&ndash;present)</span></div>
      <div class="editorial-links">
        <a class="special-issue-link" href="https://iopscience.iop.org/collections/jpd-260922-1247" target="_blank" rel="noopener noreferrer" aria-label="Journal of Physics D: Applied Physics: View special issue">View special issue <span aria-hidden="true">&#8599;</span></a>
        <a class="special-issue-link" href="https://iopscience.iop.org/collections/0022-3727_adaptive-structures-intelligent-material" target="_blank" rel="noopener noreferrer" aria-label="Journal of Physics D: Applied Physics: Earlier special issue">Earlier special issue <span aria-hidden="true">&#8599;</span></a>
      </div>
    </li>
    <li>
      <div class="editorial-details"><strong>Beilstein Journal of Nanotechnology</strong><span class="editorial-role">Guest Editor (2026&ndash;2027)</span></div>
      <div class="editorial-links">
        <a class="special-issue-link" href="https://www.beilstein-journals.org/bjnano/series/138" target="_blank" rel="noopener noreferrer" aria-label="Beilstein Journal of Nanotechnology: View special issue">View special issue <span aria-hidden="true">&#8599;</span></a>
      </div>
    </li>
    <li>
      <div class="editorial-details"><strong>Micromachines</strong><span class="editorial-role">Guest Editor (2022&ndash;present)</span></div>
      <div class="editorial-links">
        <a class="special-issue-link" href="https://www.mdpi.com/journal/micromachines/special_issues/8460C32Z5I" target="_blank" rel="noopener noreferrer" aria-label="Micromachines: View special issue">View special issue <span aria-hidden="true">&#8599;</span></a>
        <a class="special-issue-link" href="https://www.mdpi.com/journal/micromachines/special_issues/9Y03617NK9" target="_blank" rel="noopener noreferrer" aria-label="Micromachines: Earlier special issue">Earlier special issue <span aria-hidden="true">&#8599;</span></a>
      </div>
    </li>
    <li>
      <div class="editorial-details"><strong>Symmetry</strong><span class="editorial-role">Guest Editor (2021&ndash;2022)</span></div>
      <div class="editorial-links">
        <a class="special-issue-link" href="https://www.mdpi.com/journal/symmetry/special_issues/Energy_Harvesting_Metamaterials" target="_blank" rel="noopener noreferrer" aria-label="Symmetry: View special issue">View special issue <span aria-hidden="true">&#8599;</span></a>
      </div>
    </li>
    <li>
      <div class="editorial-details"><strong>ASCE Journal of Environmental Engineering</strong><span class="editorial-role">Guest Editor (2022&ndash;2023)</span></div>
      <div class="editorial-links">
        <a class="special-issue-link" href="https://ascelibrary.org/joeedu/energy-recovery-environment" target="_blank" rel="noopener noreferrer" aria-label="ASCE Journal of Environmental Engineering: View special issue">View special issue <span aria-hidden="true">&#8599;</span></a>
      </div>
    </li>
    <li>
      <div class="editorial-details"><strong>Journal of Intelligent Material Systems and Structures</strong><span class="editorial-role">Guest Editor (2024&ndash;2025)</span></div>
    </li>
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


