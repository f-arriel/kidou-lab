---
title: メンバー / People
nav:
  order: 2
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-people-group" %} メンバー / Team

{% include section.html %}

## 教授 / Principal Investigator

{% include list.html data="members" component="portrait" filter="role =~ /principal-investigator/i" %}


## 博士後期課程 / PhD Students

{% include list.html data="members" component="portrait" filter="role =~ /phd/i" %}

## 博士前期課程 / Master Students

{% include list.html data="members" component="portrait" filter="role =~ /master/i" %}

## 学部生 / Undergraduate Students

{% include list.html data="members" component="portrait" filter="role =~ /undergrad/i" %}

## 研究員 / Research Staff

{% include list.html data="members" component="portrait" filter="role =~ /research.staff/i" %}


{% include section.html %}

## 卒業生 / Alumni

お名前をクリックすると、研究テーマや学位論文のタイトルをご覧いただけます。
<br>
*Click a name to see the research theme and thesis title.*
<br><br>

{% include alumni-list.html %}


{% include section.html %}

## 就職先 / Employment of Graduates

{% assign jobs = site.employment | sort: "year" | reverse %}
{% for job in jobs %}
{{ job.degree }}　{{ job.organization }}{% if job.sector %}（{{ job.sector }}）{% endif %}
<br>
{% endfor %}



{% include section.html %}

# {% include icon.html icon="fa-solid fa-images" %} 活動写真 / Activity Photo Gallery

<br>
研究室の雰囲気や活動の様子
<br>
*Lab atmosphere and memories*
<br><br>

{% capture content %}
{% assign photos = site.gallery | sort: "date" | reverse %}
{% for photo in photos %}
{% include figure.html image=photo.image caption=photo.caption width="100%" %}
{% endfor %}
{% endcapture %}

{% include grid.html content=content %}
