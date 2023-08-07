---
title: "자격증"
layout: archive
permalink: categories/cert
author_profile: true
sidebar_main: true
---

{% assign posts = site.categories.cert %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
