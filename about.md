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

| *ISSN: 2435-2349* |  |
|:---|:------------------|
|![LLP logo](https://www.llpjournal.org/wp-content/uploads/2020/02/LLP-bold-slant.png){:width="400px"}{:.rounded}   | **Start Here!**  <br> <br> On the sidebar you can find all of our publications. <br> Alternatively, click here: <br> <br> <a class="button button--success button--rounded button--lg" href="/archive.html"><i class="far fa-play-circle"></i> To the archives </a> |


# Latest submissions

## 📔 Recent Articles and Walkthroughs

<ul>{% for post in site.posts limit: 3 %}
  {% if post.tags contains 'walkthrough' or post.tags contains 'article' %}
  <li>
    <a href="{{ post.url }}"> {{ post.title }}
    </a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🏞 Recent Playground Items

<ul>{% for post in site.posts  limit: 3 %}
  {% if post.tags contains 'playground' %}
  <li>
    <a href="{{ post.url }}"> {{ post.title }}
    </a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endfor %}
</ul>

## 🎙 Recent Podcasts
<ul>
  {% for post in site.posts %}
  {% if post.tags contains 'podcast' %}
  <li>
  <a href="{{ post.url }}">
    {{ post.title }}</a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endfor %}
</ul>

# On the web:

<a class="twitter-timeline" data-width="500" data-height="300" data-theme="dark" href="https://twitter.com/llpjournal?ref_src=twsrc%5Etfw">Tweets by llpjournal</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>