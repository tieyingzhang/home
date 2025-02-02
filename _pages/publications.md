---
layout: archive
title: "Publications (selected)"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <style>
      hr.dashed-line {
          border: 0; /* 移除默认边框 */
          border-top: 2px dashed #000; /* 设置虚线样式 */
          margin: 20px 0; /* 设置外边距 */
      }
  </style>
  <div class="wordwrap">
    <p>You can find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>. 
    <hr class="dashed-line"> <!-- 虚线 -->
    <br>Star (*) indicates that the work was conducted by my interns, or that I am the corresponding author. </p>
  </div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
