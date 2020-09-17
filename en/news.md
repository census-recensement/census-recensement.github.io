---
layout: page
title: News
lang: en
ref: news
---

<div class="archive">

  <div class="timeline" id="timeline">
    {% assign posts_by_year = site.posts | where: "lang", page.lang | group_by_exp:"post", "post.date | date: '%Y' " %}
    {% for group in posts_by_year %}
      <div class="archive-title">
        <h4 class="archive-year">{{ group.name }}</h4>
      </div>

      <ul>
      {% for post in group.items %}
        <li><div style="width:100%;float:left;">{{ post.date | date: "%B" }}</div> <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
      </ul>

    {% endfor %}
  </div>

</div>
