---
ttitle: 業績・社会貢献 / Publications & Outreach
nav:
  order: 3
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-file-signature" %} 業績 / Publications

{% include section.html %}

以下のリストは、DOIから自動生成された研究業績です。検索ボックスを利用して、キーワードで論文を絞り込むことができます。
<br>
*The following list of publications is automatically generated. You can use the search box to filter papers by keywords.*
<br><br>

{% include search-box.html %}

{% include search-info.html %}

{% include list.html data="citations" component="citation" %}


{% include section.html %}

# {% include icon.html icon="fa-solid fa-hands-holding-child" %} 社会貢献 / Social Contribution

{% assign activities = site.outreach | sort: "date" | reverse %}
{% for item in activities %}
### {{ item.title }}

{{ item.date | date: "%Y年%-m月%-d日" }}　|　{{ item.category }}{% if item.venue %}　|　{{ item.venue }}{% endif %}

{{ item.content }}
{% if item.link %}[詳細 / More information]({{ item.link }}){% endif %}

{% endfor %}
