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

{% include list.html data="members" component="portrait" filter="role =~ /Research Staff/i" %}


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
研究室の雰囲気や、懇親会・学会などの活動の様子をご紹介します。
<br>
*Introducing the atmosphere of the lab and our activities such as networking events and conferences.*
<br><br>

{% capture content %}

<!-- Note: Make sure the image files exist in your "images/people/" directory and update the captions below -->

{%
  include figure.html
  image="images/people/hanami.jpg"
  caption="花見 (Hanami) in Spring 2024."
  link="people"
  width="100%"
%}

{%
  include figure.html
  image="images/people/end_of_year_party.jpg"
  caption="End-of-year lab dinner and celebration."
  link="people"
  width="100%"
%}

{%
  include figure.html
  image="images/people/barley_field.jpg"
  caption="Fieldwork visiting the barley research plots."
  link="people"
  width="100%"
%}

{%
  include figure.html
  image="images/people/conference_2023.jpg"
  caption="Group photo at the Plant Physiology Conference 2023."
  link="people"
  width="100%"
%}

{%
  include figure.html
  image="images/people/lab_working.jpg"
  caption="Active discussion in the laboratory."
  link="people"
  width="100%"
%}

{% endcapture %}

{% include grid.html content=content %}
