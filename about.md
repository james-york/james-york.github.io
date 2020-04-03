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

## Useful links:

<ul>
  <li><a href="/2018/01/01/llp-mission.html"> Mission</a></li>
  <li><a href="/2018/01/24/reviewers.html"> Reviewers </a></li>
  <li><a href="2018/01/02/submission-guidelines.html"> Submission Guidelines </a></li>
  <li><a href="/2018/02/01/articles.html"> Articles and walkthroughs</a></li>
  <li><a href="/2018/02/01/articles.html"> About the LLP Playground!</a></li>

</ul> 

# Latest submissions

## 📔 Recent Articles and Walkthroughs

<ul>
  {% assign articles_found = 0 %}
  {% for post in site.posts %}
    {% if articles_found <= 2 %}
      {% if post.tags contains 'walkthrough' or post.tags contains 'article' %}
      {% assign articles_found = articles_found | plus: 1 %}
      <li>
        <a href="{{ post.url }}"> 📔 {{ post.title }}
        </a> [Published: {{ post.date | date_to_string }}]
      </li>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>

## 🏞 Recent Playground Items

<ul>
  {% assign playgrounds_found = 0 %}
  {% for post in site.posts %}
  {% if playgrounds_found <= 2 %}
  {% if post.tags contains 'playground' %}
  {% assign playgrounds_found = playrounds_found | plus: 1 %}
  <li>
    <a href="{{ post.url }}"> 🏞 {{ post.title }}
    </a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endif %}
  {% endfor %}
</ul>

## 🎙 Recent Podcasts
<ul>
  {% assign pods_found = 0 %}
  {% for post in site.posts %}
  {% if pods_found <= 2 %}
  {% if post.tags contains 'podcast' %}
  {% assign pods_found = pods_found | plus: 1 %}
  <li>
  <a href="{{ post.url }}"> 🎙
    {{ post.title }}</a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endif %}
  {% endfor %}
</ul>

# On the web:

<a class="twitter-timeline" data-width="500" data-height="300" data-theme="dark" href="https://twitter.com/llpjournal?ref_src=twsrc%5Etfw">Tweets by llpjournal</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>