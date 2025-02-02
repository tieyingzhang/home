---
layout: archive
title: "Publications (selected)"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <style>
    .dashed-line {
      height: 2px; /* 设置虚线高度 */
      background: repeating-linear-gradient(
        to right,
        #000, /* 虚线颜色 */
        #000 5px, /* 虚线长度 */
        transparent 5px, /* 透明间隔 */
        transparent 10px /* 间隔长度 */
      );
      margin: 20px 0; /* 设置外边距 */
    }
  </style>
  <div class="wordwrap">
    <p>You can find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>. 
    <hr class="simple-dashed-line"> <!-- 简单虚线横线 -->
    <br>Star (*) indicates that the work was conducted by my interns, or that I am the corresponding author. </p>
  </div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
