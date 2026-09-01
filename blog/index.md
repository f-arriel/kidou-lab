---
title: お知らせ / News
nav:
  order: 4
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-bullhorn" %} お知らせ / News

{% include section.html %}

木藤研究室からの最新情報や研究室の日常をお届けします。キーワードやタグを使って記事を検索できます。
<br>
*Latest updates and daily life from the Kidou Laboratory. You can search for articles using keywords or tags.*
<br><br>

{% include search-box.html %}

{% include tags.html tags=site.tags %}

{% include search-info.html %}

{% include list.html data="posts" component="post-excerpt" %}
