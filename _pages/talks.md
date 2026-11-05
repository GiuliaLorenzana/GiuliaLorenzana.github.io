---
layout: page
permalink: /talks/
title: Talks
description:
nav: true
nav_order: 2
---

<!-- _pages/talks.md — content lives in _data/talks.yml -->
<div class="publications">
{% for s in site.data.talks %}
  <h2 class="year">{{ s.section }}</h2>
  <ol class="bibliography">
  {% for t in s.talks %}
    <li>
      <div class="row">
        <div class="col-sm-2 abbr"></div>
        <div class="col-sm-8">
          <div class="title">{{ t.title }}</div>
          <div class="author">{{ t.date }}</div>
          <div class="periodical"><em>{{ t.venue }}</em></div>
          {% if t.video %}
            <div class="links">
              <a href="{{ t.video }}" class="btn btn-sm z-depth-0" role="button" rel="external nofollow noopener" target="_blank">Video</a>
            </div>
          {% endif %}
        </div>
      </div>
    </li>
  {% endfor %}
  </ol>
{% endfor %}
</div>
