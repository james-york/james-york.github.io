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

## 🤝 Join us!
<table>
	<tr>
		<th><a href="http://bit.ly/LLPSlack"><img alt="!!!!!!!!!!!!!!" src="/assets/images/llp-join-slack-image.png" height="250"></a><br> Main communication hub</th>
		<th><iframe src="https://discordapp.com/widget?id=523277560809783297&theme=dark" width="250" height="250" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe> <br> Used for conferences </th>
	</tr>
</table>

## 🔗 Useful links

<table>
  <tr>
    <th><a href="/2018/01/01/llp-mission.html"> Mission</a></th>
    <th><a href="/2020/06/23/llp-inclusivity-statement.html"> Inclusivity Statement</a></th>
    <th><a href="2018/01/02/submission-guidelines.html"> Submission Guidelines </a></th>
    <th><a href="/2018/02/01/articles.html"> Articles and walkthroughs</a></th>
    <th><a href="/2020/04/04/playground-landing.html"> About the LLP Playground</a></th>
  </tr>
 </table>

 
# 🆕 Latest releases

## 🏞 Recent Playground Items

<ul>
  {% assign playgrounds_found = 0 %}
  {% for post in site.posts %}
    {% if playgrounds_found <= 2 %}
  {% if post.tags contains 'playground' %}
  {% assign playgrounds_found = playgrounds_found | plus: 1 %}
  <li>
    <a href="{{ post.url }}"> 🏞 {{ post.title }}
    </a> [Published: {{ post.date | date_to_string }}]
  </li>
  {% endif %}
  {% endif %}
  {% endfor %}
</ul>

<a class="button button--success button--rounded button--lg" href="/2018/02/01/playground-items.html"><i class="far fa-play-circle"></i> 🏞 All playground items </a>

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

<a class="button button--success button--rounded button--lg" href="/2018/02/01/articles.html"><i class="far fa-play-circle"></i> 📔 All articles and walkthroughs </a>

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


# 🌐 On the web

<a class="twitter-timeline" data-width="500" data-height="300" data-theme="dark" href="https://twitter.com/llpjournal">Tweets by llpjournal</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>