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

</style>
### Journal Articles (Upadated on 2026.01.08)


#### 2026

{% assign sorted_articles = site.data.article2026 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2025

{% assign sorted_articles = site.data.article2025 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2024

{% assign sorted_articles = site.data.article2024 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2023

{% assign sorted_articles = site.data.article2023 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2022

{% assign sorted_articles = site.data.article2022 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2021

{% assign sorted_articles = site.data.article2021 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2020

{% assign sorted_articles = site.data.article2020 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2019

{% assign sorted_articles = site.data.article2019 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2018

{% assign sorted_articles = site.data.article2018 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2017

{% assign sorted_articles = site.data.article2017 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" class="doi-link" target="_blank" rel="noopener noreferrer">[DOI]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" class="pdf-link" target="_blank" rel="noopener noreferrer">[PDF]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" class="si-link" target="_blank" rel="noopener noreferrer">[SI]</a>{% endif %}</p>
{% endfor %}

#### 2016

{% assign sorted_articles = site.data.article2016 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p class="pub-entry"><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. {% if item.Doi %}<a href="{{ item.Doi }}" target="_blank" rel="noopener noreferrer">[doi]</a>{% endif %}{% if item.PDF %} <a href="{{ item.PDF | prepend: site.baseurl }}" target="_blank" rel="noopener noreferrer">[pdf]</a>{% endif %}{% if item['Supplementary Information'] %} <a href="{{ item['Supplementary Information'] }}" target="_blank" rel="noopener noreferrer">[supplementary]</a>{% endif %}</p>
{% endfor %}
