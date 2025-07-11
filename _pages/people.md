---
permalink: /people/
title: "People"
layout: home
author_profile: true
---

Our lab brings together researchers passionate about creating intelligent systems that meaningfully interact with humans. We work at the intersection of Human-Computer Interaction, Data Visualization, and Artificial Intelligence.

{% assign people = site.data.people  %}

{% assign faculty = people | where: "role", "faculty" %}
{% assign phd = people | where: "role", "phd" %}
{% assign masters = people | where: "role", "masters" %}
{% assign undergrad = people | where: "role", "undergrad" %}
{% assign alumni = people | where: "role", "alumni" %}

{% assign lab = faculty | concat: phd | concat: masters | concat: undergrad | concat: alumni %}
{% include people-list.html arr=lab %}
