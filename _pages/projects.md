---
layout: archive
title: "Selected Projects"
permalink: /projects/
author_profile: true
toc: true
---
{% include base_path %}
{% assign sortedProjects = site.projects | sort: 'date' | reverse %}

This page contains a selection of my current and previous research/course/toy projects, categorized by topic. --- _Last updated in March 2025_.

## Photoacoustic probe design 
---

Current research project: ultrasound image-guided needle insertion. <br/>
More details to be disclosed as the project progresses.


## An umbrella-inspired snap-on robotic 3D photoacoustic endoscopic probe for augmented intragastric sensing
---

{% for post in sortedProjects %}
  {% if post.topic == 'robot-assisted_imaging' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## FR5 robotic arm fully automatic photoacoustic scanning palm arm image reconstruction
---

{% for post in sortedProjects %}
  {% if post.topic == 'marine_robotics' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## In vivo photoacoustic scanning using a flexible robot equipped with a micro-photoacoustic probe
---

{% for post in sortedProjects %}
  {% if post.topic == 'bio-inspired_robotics' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}



