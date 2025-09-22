---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* University of Texas at Austin (USA)
  * Ph.D. in Marketing, McCombs School of Business, 2028 (expected)

* Fudan University (China)
  * Researh Training, Management, School of Management, 2021

* University of Iowa (USA)
  * Visiting Scholar, Marketing, Tippie College of Business, 2020
 
* Xiamen University (China)
  * Bachelor of Economics, School of Economics, 2014

Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
