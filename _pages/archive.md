---
layout: inner
title: Archive
permalink: /archive/
---

<div class="row">
  <div class="column">
  <h3>News Archive</h3>

    <div class="row">
      <div class="column">
      {% for post in site.posts %}
        <h4><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h4>
        <p>{{ post.content | truncatewords:50 }}</p>
      {% endfor %}
      