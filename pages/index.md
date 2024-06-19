---
layout: default
id: home
---

<link rel="alternate" type="application/rss+xml" href="{{ site.url }}/feed.xml">
# Welcome to My Blog!

<div class="infobox">
This blog is written with best intentions, please be favorable when you read it.
</div>

<div class="infobox">
While most things should be in English some posts will be in German because I do not have the sometimes necessary feeling for nuances in English.
</div>

## Latest Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}


<div style="display: flex; flex-wrap: wrap;">
  {% assign featured_images = site.data.images | where: "featured", true %}
  {% for item in featured_images limit:5 %}
  <div style="margin: 10px;">
    <div style="max-width: 150px; height: auto;">{{item.img}}</div>
    <p>{{ item.description }}</p>
  </div>
  {% endfor %}
</div>

---

Last updated {{ site.time | date: "%Y-%m-%d %H:%M:%S" }}