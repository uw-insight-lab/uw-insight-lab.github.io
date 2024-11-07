---
permalink: /people/
title: "People"
layout: home
author_profile: true
---

{% assign people = site.data.people  %}

{% include people-list.html arr=people title="" %}
