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

{% include list.html data="members" component="portrait" filter="role =~ /research-staff/i" %}


{% include section.html %}

## 卒業生 / Alumni
永井里美
<br>
鵜飼真美生
<br>
久保岳人
<br>
横山悠理

{% include section.html %}

# {% include icon.html icon="fa-solid fa-images" %} 活動写真 / Activity Photo Gallery

<br>
研究室の雰囲気や活動の様子をご紹介します。
<br>
*Lab atmosphere and activities*
<br><br>

{% capture content %}

<!-- Note: Make sure the image files exist in your "images/people/" directory and update the captions below -->

{% capture content %}
  {% assign photos = site.gallery | sort: "date" | reverse %}
  {% for photo in photos %}
    {% include figure.html image=photo.image caption=photo.caption width="100%" %}
  {% endfor %}
{% endcapture %}

{% include grid.html content=content %}
