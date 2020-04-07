---
layout: article
title: Playground Items
key: playground-items
show_title: false
pageview: true
sidebar:
  nav: docs-en
aside:
  toc: true
sharing: false
---

The LLP Playground is full of amazing teaching and research items which can be shared, discussed, and *peer-reviewed.*

<a class="button button--success button--rounded button--lg" href="/2020/04/04/about-the-playground.html"><i class="far fa-play-circle"></i> Learn more here </a>


# 🏞 Playground items by date

<ul>
  {% for post in site.posts %}
  {% if post.tags contains 'playground' %}
  <li>
  <a href="{{ post.url }}">
    <p><b>{{ post.title }}</b></p></a>
    <p>Published: {{ post.date | date_to_string }}</p> 
  </li>
  {% endif %}
  {% endfor %}
</ul>