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
comments: false
---

A playground presents **methods**, **materials**, **concepts** or **experiences** based in **practice** and grounded in *theory* that can serve to *inform*, *inspire* or *challenge* practitioners and/or researchers. How a playground is based in practice, and how it is grounded in theory, can then be very individual, as long as these two things are given. There must be value in it for the reader, not only for the author.

The LLP Playground is full of amazing teaching and research items which can be shared, discussed, and *peer-reviewed.*

<a class="button button--success button--rounded button--lg" href="/2020/04/04/about-the-playground.html"><i class="far fa-play-circle"></i> Learn more here </a>


# 🏞 Playground items by date

<ul>
  {% for post in site.posts %}
    {% if post.tags contains 'playground' %}
      <li>
        <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
        <p>Published: {{ post.date | date_to_string }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
