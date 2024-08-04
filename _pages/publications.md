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

.btn-container {
    margin-top: -15px;
    display: flex; /* 使用flex布局 */
    gap: 10px; /* 设置按钮之间的间距 */
}

.btn {
    display: inline-block;
    padding: 2px 5px;
    margin: 3px 2;
    font-size: 14px;
    font-weight: bold;
    color: white;
    border-radius: 5px;
    text-align: center;
    text-decoration: none;
}

.btn-doi {
    background-color: #f44336; /* 红色 */
    }

.btn-pdf {
    background-color: #008CBA; /* 蓝色 */
}

.btn-supplementary {
    background-color: #4CAF50; /* 绿色 */
}
</style>

#### Publications 2024

{% assign sorted_articles = site.data.article2024 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2023

{% assign sorted_articles = site.data.article2023 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2022

{% assign sorted_articles = site.data.article2022 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2021

{% assign sorted_articles = site.data.article2021 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2020

{% assign sorted_articles = site.data.article2020 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2019

{% assign sorted_articles = site.data.article2019 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2018

{% assign sorted_articles = site.data.article2018 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2017

{% assign sorted_articles = site.data.article2017 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}

#### Publications 2016

{% assign sorted_articles = site.data.article2016 %}

{% for item in sorted_articles %}
<a name="J{{ item.index }}"></a>
<p><strong>[J{{ item.index }}]</strong> [{{ item.published }}] {% for author in item.authors %}{% if author == "Hu, Guobiao" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% if forloop.last == false %}, {% endif %}{% endfor %}, “{{ item.title }}”, <strong>{{ item.journal }}</strong>. </p>
<div class="btn-container">
{% if item.Doi %}
<a href="{{ item.Doi }}" class="btn btn-doi">DOI</a>
{% endif %}
{% if item.PDF %}
<a href="{{ item.PDF | prepend: site.baseurl }}" class="btn btn-pdf">PDF</a>
{% endif %}
{% if item['Supplementary Information'] %}
<a href="{{ item['Supplementary Information'] }}" class="btn btn-supplementary">SUPPLEMENTARY</a>
{% endif %}
</div>
{% endfor %}