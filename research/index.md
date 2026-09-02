---
title: 研究内容 / Research
nav:
  order: 1
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-microscope" %} 研究内容 / Research

{% include section.html %}

## 現在の研究テーマ / Current Research

{% assign current = site.themes | where: "status", "current" | sort: "order" %}
{% for theme in current %}
{% include feature.html image=theme.image title=theme.title text=theme.content %}
{% endfor %}

{% include section.html %}

## これまでの研究テーマ / Past Research

{% assign past = site.themes | where: "status", "past" | sort: "order" %}
{% for theme in past %}
{% include feature.html image=theme.image title=theme.title text=theme.content %}
{% endfor %}

