---
title: ""                         # hide big page header
permalink: /research/
layout: archive
author_profile: true
entries_layout: list
show_excerpts: true
classes: hide-title
---

{% include base_path %}

## Publications
{% assign pubs = site.research | where_exp: "item", "item.categories contains 'publications'" | sort: "date" | reverse %}
{% for post in pubs %}
{% include archive-single.html %}
{% endfor %}

---

## Working Papers
<div class="nolink-titles">
{% assign wps = site.research | where_exp: "item", "item.categories contains 'working-papers'" | sort: "date" | reverse %}
{% for post in wps %}
{% include archive-single.html %}
{% endfor %}
</div>

---

## Selected Work in Progress
<div class="nolink-titles">
{% assign wip = site.research | where_exp: "item", "item.categories contains 'wip'" | sort: "date" | reverse %}
{% for post in wip %}
{% include archive-single.html %}
{% endfor %}
</div>
