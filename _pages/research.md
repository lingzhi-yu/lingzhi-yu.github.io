---
title: ""
permalink: /research/
layout: archive
author_profile: true
entries_layout: list
show_excerpts: true
classes: hide-title
---

{% include base_path %}

## Publications
<div class="pubs-section">
{% assign pubs = site.research | where_exp: "item", "item.categories contains 'publications'" | sort: "date" | reverse %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}
</div>

---

## Working Papers
<div class="wp-section">
{% assign wps = site.research | where_exp: "item", "item.categories contains 'working-papers'" | sort: "date" | reverse %}
{% for post in wps %}
  <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
    <h2 class="archive__item-title no_toc">{{ post.title }}</h2>
    {% if post.excerpt %}
      <div class="archive__item-excerpt" itemprop="description">
        {{ post.excerpt | markdownify }}
      </div>
    {% endif %}
  </article>
{% endfor %}
</div>

---

## Selected Work in Progress
<div class="wip-section">
{% assign wip = site.research | where_exp: "item", "item.categories contains 'wip'" | sort: "date" | reverse %}
{% for post in wip %}
  <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
    <h2 class="archive__item-title no_toc">{{ post.title }}</h2>
    {% if post.excerpt %}
      <div class="archive__item-excerpt" itemprop="description">
        {{ post.excerpt | markdownify }}
      </div>
    {% endif %}
  </article>
{% endfor %}
</div>
