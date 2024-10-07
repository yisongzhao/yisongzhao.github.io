---
layout: archive
title: "Selected Projects"
permalink: /projects/
author_profile: true
toc: true
---
{% include base_path %}
{% assign sortedProjects = site.projects | sort: 'date' | reverse %}

This page contains a selection of my current and previous research/course/toy projects, categorized by topic. --- _Last updated in October 2024_.

## Image-Guided Robotic Interventions
---

Current research project: ultrasound image-guided needle insertion. <br/>
More details to be disclosed as the project progresses.


## Robot-Assisted Imaging
---

{% for post in sortedProjects %}
  {% if post.topic == 'robot-assisted_imaging' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Marine Robotics
---

{% for post in sortedProjects %}
  {% if post.topic == 'marine_robotics' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Bio-Inspired Robotics
---

{% for post in sortedProjects %}
  {% if post.topic == 'bio-inspired_robotics' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Others
---

{% for post in sortedProjects %}
  {% if post.topic == 'others' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


