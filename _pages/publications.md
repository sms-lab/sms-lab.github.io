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
.pub-entry { display: flex; flex-wrap: wrap; align-items: flex-start; justify-content: space-between; gap: 0.75rem; margin-bottom: 0.8rem; }
.pub-text { flex: 1 1 0; min-width: 0; }
.dim-count { display: flex; align-items: flex-start; flex-shrink: 0; margin-left: 0.8rem; padding-top: 0.12rem; }
.dim-count .__dimensions_badge_embed__ { display: inline-flex; transform-origin: center center; }
.cover-grid {
  display: grid;
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 1.2rem;
  margin: 1rem 0 2.2rem;
}
.cover-item {
  display: block;
}
.cover-item img {
  display: block;
  width: 100%;
  aspect-ratio: 3 / 4;
  object-fit: cover;
  border-radius: 0;
  box-shadow: 0 0.25rem 0.9rem rgba(0, 0, 0, 0.16);
}
@media (max-width: 767px) {
  .pub-entry { align-items: stretch; }
  .dim-count { margin-left: 0; width: 100%; justify-content: flex-start; }
  .cover-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 0.9rem; }
}

</style>
### Cover Articles

<div class="cover-grid" markdown="0">
<div class="cover-item">
<img src="{{ '/images/Cover/Device 4 (2025) 100903.jpg' | relative_url }}" alt="Device 4 (2025) 100903 cover">
</div>
<div class="cover-item">
<img src="{{ '/images/Cover/Joule 10 (2026) 102338.jpg' | relative_url }}" alt="Joule 10 (2026) 102338 cover">
</div>
</div>

### Journal Articles (Updated on 2026-09-30)

{% assign year_files = "article2026,article2025,article2024,article2023,article2022,article2021,article2020,article2019,article2018,article2017,article2016" | split: "," %}

{% for datafile in year_files %}
{% assign sorted_articles = site.data[datafile] %}
{% if sorted_articles %}
{% assign year = datafile | remove: "article" %}
### {{ year }}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry">
  <span class="pub-text"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF and item.PDF != 'Not available' and item.PDF != '' %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</span>
  <span class="dim-count">{% if item.doi %}<span class="__dimensions_badge_embed__" data-doi="{{ item.doi }}" data-style="small_rectangle" data-legend="hover-right"></span>{% else %}&nbsp;{% endif %}</span>
</p>
{% endfor %}

{% endif %}
{% endfor %}

<script async src="https://badge.dimensions.ai/static/ai/badge.js" charset="utf-8"></script>
