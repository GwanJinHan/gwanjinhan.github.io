---
title: "Nomad Coders"
layout: archive
permalink: categories/nomadcoders
author_profile: true
sidebar_main: true
---

{% assign posts = site.categories.nomadcoders %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
