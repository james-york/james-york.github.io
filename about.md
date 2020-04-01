---
layout: article
titles:
  # @start locale config
  en      : &EN       About
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  关于
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  關於
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       소개
  ko-KR   : *KO
  fr      : &FR       À propos
  fr-BE   : *FR
  fr-CA   : *FR
  fr-CH   : *FR
  fr-FR   : *FR
  fr-LU   : *FR
  # @end locale config
key: page-about
show_title: false
sidebar:
  nav: docs-en
aside:
  toc: true
---

![LLP logo](https://www.llpjournal.org/wp-content/uploads/2020/02/LLP-bold-slant.png){:width="400px"}{:.rounded}

# 👈 Start here

On the sidebar you can find all of the playground publications. Alternatively, click the button below:

<a class="button button--success button--rounded button--lg" href="/archive.html"><i class="far fa-play-circle"></i> To the archives </a>

# Latest submissions

## 📔 Recent Articles and Walkthroughs

<ul>{% for post in site.posts limit: 3 %}
  {% if post.tags contains 'walkthrough' or post.tags contains 'article' %}
  <li>
    <a href="{{ post.url }}"> {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🏞 Recent Playground Items

<ul>{% for post in site.posts  limit: 3 %}
  {% if post.tags contains 'playground' %}
  <li>
    <a href="{{ post.url }}"> {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🎙 Recent Podcasts

<ul>{% for post in site.posts  limit: 3 %}
  {% if post.tags contains 'podcast' %}
  <li>
    <a href="{{ post.url }}"> {{ post.title }}
    </a>
  </li>
  {% endif %}
  {% endfor %}
</ul>