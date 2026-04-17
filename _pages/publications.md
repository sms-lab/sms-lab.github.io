---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
---

<style>
.jumbotron {
    padding: 3%;
    padding-bottom: 10px;
    padding-top: 10px;
    margin-top: 10px;
    margin-bottom: 30px;
}

.pub-entry a {
    text-decoration: underline;
}

.doi-link { color: rgb(0,157,255); font-weight: bold; text-decoration: none; }
.pdf-link { color: rgb(192,0,0); font-weight: bold; text-decoration: none; }
.si-link { color: rgb(112,48,160); font-weight: bold; text-decoration: none; }
.pub-entry { display: flex; align-items: center; justify-content: space-between; gap: 0.75rem; margin-bottom: 0.8rem; }
.pub-text { flex: 1; min-width: 0; }
.dim-count { display: flex; align-items: center; flex-shrink: 0; margin-left: 0.8rem; }
.dim-count .__dimensions_badge_embed__ { display: inline-flex; transform: scale(0.8); transform-origin: center center; }

</style>
### Journal Articles (Upadated on 2026-04-18)

{% assign year_files = "article2026,article2025,article2024,article2023,article2022,article2021,article2020,article2019,article2018,article2017,article2016" | split: "," %}

{% for datafile in year_files %}
{% assign sorted_articles = site.data[datafile] %}
{% if sorted_articles %}
{% assign year = datafile | remove: "article" %}
#### {{ year }}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry">
  <span class="pub-text"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</span>
  <span class="dim-count">{% if item.doi %}<span class="__dimensions_badge_embed__" data-doi="{{ item.doi }}" data-style="small_circle" data-legend="hover-right"></span>{% else %}&nbsp;{% endif %}</span>
</p>
{% endfor %}

{% endif %}
{% endfor %}

<script async src="https://badge.dimensions.ai/static/ai/badge.js" charset="utf-8"></script>
