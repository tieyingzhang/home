---
layout: archive
title: "Publications (selected)"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">
    You can find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.
    
    Star (*) indicates that the work was conducted by interns under my supervision, or that I am the corresponding author.
  </div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
