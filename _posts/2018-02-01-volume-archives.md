---
layout: article
title: Volume Archives
key: volume-archives
tags:
- meta
show_title: false
pageview: true
sidebar:
  nav: docs-en
aside:
  toc: true
sharing: false
comments: false
---

# 🏦 Volumes by date

<ul>
  {% assign sorted_posts = site.posts | sort: 'title' | reverse %}
  {% for post in  sorted_posts %}
  {% if post.tags contains 'volume archive' %}
  <li>
  <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
  </li>
  {% endif %}
  {% endfor %}
</ul>

--- 
# All published papers by type

## 📔 Articles
<ul>
  {% assign sorted_posts = site.posts | reverse %}
  {% for post in sorted_posts %}
  {% if post.tags contains 'article' %}
  <li>
  <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
    <p><b>Published:</b> {{ post.date | date_to_string }}</p> 
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🚶‍♂️ Walkthroughs
<ul>
  {% assign sorted_posts = site.posts | reverse %}
  {% for post in sorted_posts %}
  {% if post.tags contains 'walkthrough' %}
  <li>
  <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
    <p><b>Published:</b> {{ post.date | date_to_string }}</p> 
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🏞 Playgrounds
<ul>
  {% assign sorted_posts = site.posts | reverse %}
  {% for post in sorted_posts %}
  {% if post.tags contains 'playground' %}
  <li>
  <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
    <p><b>Published:</b> {{ post.date | date_to_string }}</p> 
  </li>
  {% endif %}
  {% endfor %}
</ul>