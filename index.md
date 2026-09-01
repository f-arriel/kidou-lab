---
---

<div style="text-align: center; margin-top: 20px; margin-bottom: 30px;">
  <h1 style="margin-bottom: 5px; font-size: 2.5em;">木藤研 - Kidou Lab</h1>
  <p style="text-align: center; "font-size: 1.25em; color: var(--primary); font-weight: 500; margin-top: 0;">
    植物生命科学 - Plant Physiology and Molecular Biology
  </p>
</div>

{% include section.html %}

<!-- MODERN, SCROLLABLE NEWS SECTION START -->
<div style="
  max-width: 900px;
  margin: 0 auto 40px auto;
  border-radius: 8px;
  background-color: var(--background);
  border: 1px solid var(--light-gray);
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  overflow: hidden;
">
  <!-- News Header (Centered) -->
  <div style="
    padding: 15px 20px;
    background-color: var(--background-alt);
    border-bottom: 1px solid var(--light-gray);
    text-align: center;
  ">
    <h3 style="margin: 0; font-size: 1.4em;">
      {% include icon.html icon='fa-solid fa-satellite-dish' %}
      研究室ニュース / Lab News
    </h3>
  </div>

  <!-- Scrollable Feed Container (Fixed Height) -->
  <div style="
    height: 300px; /* Adjust height here as needed */
    overflow-y: auto; /* Enables inner vertical scroll */
    padding: 10px 20px;
    scrollbar-width: thin; /* Clean modern scrollbar for Firefox */
    scrollbar-color: var(--gray) var(--background-alt); /* Colors for scrollbar */
  ">
    <!-- Jekyll Post Loop: Fetches most recent 10 posts -->
    {% assign recent_posts = site.posts | limit: 10 %}
    {% if recent_posts.size > 0 %}
      <ul style="list-style-type: none; padding: 0; margin: 0;">
        {% for post in recent_posts %}
          <li style="
            border-bottom: 1px solid var(--light-gray);
            padding: 15px 5px;
            display: flex;
            align-items: flex-start;
          ">
            <!-- Modern Date Badge (Left Side) -->
            <div style="
              text-align: center;
              margin-right: 20px;
              flex-shrink: 0;
              width: 90px;
              font-family: var(--code);
            ">
              <span style="font-size: 0.9em; font-weight: 600;">{{ post.date | date: "%Y年" }}</span><br>
              <span style="color: var(--primary); font-size: 1.1em; font-weight: 600; line-height: 1;">{{ post.date | date: "%m/%d" }}</span>
            </div>

            <!-- Post Title (Clickable) -->
            <div style="flex-grow: 1; padding-top: 2px;">
              <a href="{{ post.url | relative_url }}" style="font-weight: 500; font-size: 1.1em; text-decoration: none; color: inherit;">
                {{ post.title }}
              </a>
            </div>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <!-- Fallback message if no posts exist -->
      <div style="text-align: center; padding: 40px; color: var(--gray);">
        現在、新しいニュースはありません。<br>
        *There are currently no new announcements.*
      </div>
    {% endif %}
  </div>

  <!-- Bottom Link to full Blog page -->
  <div style="
    padding: 10px;
    text-align: center;
    border-top: 1px solid var(--light-gray);
    background-color: var(--background-alt);
  ">
    <a href="{{ '/blog/' | relative_url }}" style="font-size: 0.9em;">
      すべての投稿を見る / See all posts {% include icon.html icon='fa-solid fa-angles-right' %}
    </a>
  </div>
</div>
<!-- MODERN, SCROLLABLE NEWS SECTION END -->

{% include section.html %}

## 木藤研究室へようこそ - Welcome to Kidou Lab

遺伝子やタンパク質の機能解析を通じて、あなたも美しい生命現象の謎解きに参加しませんか？
<br>
Join us in unraveling the beautiful mysteries of life phenomena through the functional analysis of genes and proteins.
<br><br>
オオムギは、ビールやウイスキーの主原料として利用されているだけでなく、日本では麦茶や麦ご飯としても利用されています。また、食物繊維であるβ-グルカンを豊富に含むことから、健康食品としても着目されています。また、オオムギは低温をはじめとする環境ストレスに耐性を持つことから、コムギの栽培に適さない寒冷地である北欧でも栽培できるという特徴を持っています。私たちの研究室では、このオオムギが持つ低温耐性の仕組みとβ-グルカンを合成する仕組みを分子レベルで解き明かす研究に着手しています。また、モデル植物であるシロイヌナズナを用いて、花芽形成の研究にも挑んでいます。教員が一人しかいない小さな研究室ですが、地道に植物の生理機構を分子レベルで解き明かす研究に取り組んでいます。植物に興味がある方は、是非私たちの研究室のメンバーに加わって下さい。
<br><br>
Barley is not only used as a main ingredient in beer and whiskey, but is also enjoyed in Japan as barley tea and barley rice. Additionally, because it is rich in the dietary fiber β-glucan, it is attracting attention as a health food. Barley is also highly tolerant to environmental stresses, particularly cold temperatures, allowing it to be cultivated in cold regions like Northern Europe where wheat cannot thrive. In our laboratory, we are working to unravel the molecular mechanisms behind barley's cold tolerance and β-glucan synthesis. We are also conducting research on floral bud formation using the model plant *Arabidopsis thaliana*. Although we are a small laboratory, we are working to elucidate the physiological mechanisms of plants at the molecular level. If you have an interest in plants, we warmly invite you to join our team!

<br>
<img src="{{ '/images/Home.jpg' | relative_url }}" alt="Kidou Laboratory" style="display: block; margin: 0 auto; width: 100%; max-width: 900px; border-radius: 8px;">
