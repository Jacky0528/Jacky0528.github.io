---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{ site.author.googlescholar }}" class="no-link">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<div class="publications-list">
  {% for post in site.publications reversed %}
    <div class="publication">
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt }}</p>
    </div>
  {% endfor %}
</div>

<style>
.publications-list .publication h2 {
  pointer-events: none;
  cursor: default;
  text-decoration: none;
  color: inherit;
}
</style>
