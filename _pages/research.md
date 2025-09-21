---
title: "Research"
permalink: /research/
layout: archive
author_profile: true
entries_layout: list
show_excerpts: true
---

{% include base_path %}

## Publications
{% assign pubs = site.research | where_exp: "item", "item.categories contains 'publications'" | sort: "date" | reverse %}
{% for post in pubs %}
{% include archive-single.html %}
{% endfor %}

---

## Working Papers
{% assign wps = site.research | where_exp: "item", "item.categories contains 'working-papers'" | sort: "date" | reverse %}
{% for post in wps %}
{% include archive-single.html %}
{% endfor %}

---

## Selected Work in Progress
{% assign wip = site.research | where_exp: "item", "item.categories contains 'wip'" | sort: "date" | reverse %}
{% for post in wip %}
{% include archive-single.html %}
{% endfor %}
