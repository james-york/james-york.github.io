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

{% include carousel.html height="32" unit="%" duration="3" %} 

*ISSN: 2435-2349* 


 <style>
         table, td, th {
            text-align: center;
         }
         button {
          text-align: center;
      </style>

## 🔗 Useful links

<table>
  <tr>
    <th>
      <script type='text/javascript' src='https://storage.ko-fi.com/cdn/widget/Widget_2.js'></script><script type='text/javascript'>kofiwidget2.init('Check out the LLP store', '#867ade', 'F1F6HOTID');kofiwidget2.draw();</script>
    </th>
    <th>
      <a class="button button--success button--rounded button--md" href="/2018/01/01/contact-us.html#-newsletter">💌 Newsletter</a>
    </th>
    <th>
      <a class="button button--success button--rounded button--md" href="/2018/01/01/llp-mission.html">Mission</a>
    </th>
  </tr>
  <tr>
    <th>
      <a class="button button--success button--rounded button--md" href="2018/01/02/submission-guidelines.html">Submission Guidelines</a>
    </th>
    <th>
      <a class="button button--success button--rounded button--md" href="/2020/04/04/playground-landing.html">About the LLP Playground</a>
    </th>
    <th>
      <a class="button button--success button--rounded button--md" href="/2020/06/23/llp-inclusivity-statement.html">Inclusivity Statement</a>
    </th>
  </tr>
  </table>



# 👇 Read these papers first 

If you want to get a good grounding on what LLP is, we recommend starting with these three papers. Let us know what you think on the [LLP Discord](https://discord.gg/je9QZsnntf).

1. [One game, many approaches: How teachers can use a single game with any teaching methodology](https://llpjournal.org/2021/09/21/spano-one-game-to-rule-them-all.html)
2. [Teaching language and literacy with the pedagogy of multiliteracies: simplified here for teachers and students](https://llpjournal.org/2022/05/11/dehaan-teaching-language-and-literacy-with-games-simplified-for-teachers.html)
3. [How to teach languages with Among Us](https://llpjournal.org/2020/10/25/j-york-how-to-teach-languages-with-among-us.html)

 
# 🆕 Latest publications
<ul>
  {% assign articles_found = 0 %}
  {% for post in site.posts %}
  {% if articles_found <= 4 %}
    {% if post.tags contains 'playground' or post.tags contains 'article' or post.tags contains 'walkthrough' or post.tags contains 'llpx-symposium-2025' %}
      {% assign articles_found = articles_found | plus: 1 %}
     {% if post.tags contains 'playground' %}
        {% assign tagger = "🏞" %}
      {% endif %}
      {% if post.tags contains 'walkthrough' %}
        {% assign tagger = "🚶" %}
      {% endif %}
      {% if post.tags contains 'article' %}
        {% assign tagger = "📔" %}
      {% endif %}
      <li>
        {{tagger}} <a href="{{ post.url }}">{{ post.title }}
        </a> [Published: {{ post.date | date_to_string }}]
      </li>
    {% endif %}
  {% endif %}
  {% endfor %}
</ul>

<a class="button button--success button--rounded button--lg" href="/2018/02/01/playground-items.html"><i class="far fa-play-circle"></i> 🏞 All playground items </a> 
<a class="button button--success button--rounded button--lg" href="/2018/02/01/articles.html"><i class="far fa-play-circle"></i> 📔 All articles and walkthroughs </a>

## 🤝 Join us!
<table>
  <tr>
    <th>
      LLP is not only a journal, but a community of practice. We use Discord as "our place to talk and hang out." Participate in discussions such as:
      <ul>
      <li>Introduce your LLP context, </li>
      <li>Receive advice from practicing LLPers,</li>
      <li>Propose and collaborative research projects,</li>
      <li>Discuss topics related to games, play, language teaching, pedagogy and more,</li>
      <li>Stay up to date regarding reviewing opportunities (such as any 🆕 <a href="/2018/01/02/submission-guidelines.html#-playground-items-easy-mode">playground</a> submissions).</li></ul>
    </th>
    <th>Join our Discord community here: <iframe src="https://discordapp.com/widget?id=523277560809783297&theme=dark" width="250" height="250" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe></th>
  </tr>
</table>

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

# 🏦 Previous Volumes

<ul>
  {% for post in site.posts %}
  {% if post.tags contains 'volume archive' %}
  <li>
    <a href="{{ post.url }}"> <b>{{ post.title }}</b></a>
  </li>
  {% endif %}
  {% endfor %}
</ul>