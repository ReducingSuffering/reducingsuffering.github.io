---
layout: blog
title: "Reducing Suffering: авторы и источники"
---
<h2>Авторы по количеству записей</h2>
{% assign authors = site.posts | map: 'authors' | uniq %}
{% for author in authors %}{% if author %}{% assign count = 0 %}{% for post in site.posts %}{% if post.authors contains author %}{% assign count = count | plus: 1 %}{% endif %}{% endfor %}<span class="post-tags-inline"><a href="#{{ author }}" style="font-size: {% if count > 1 %}{{ count | times: 4 | plus: 105 | at_most: 180 }}{% else %}90{% endif %}%">{{ author | replace: " ", "&nbsp;" }}&nbsp;({{ count }})</a></span>{% else %}&nbsp;{% endif %}
{% endfor %}

---

<h2>Источники по количеству записей</h2>
{% assign sources = site.posts | map: 'source' | uniq %}
{% for source in sources %}{% if source %}{% assign count = 0 %}{% for post in site.posts %}{% if post.source contains source %}{% assign count = count | plus: 1 %}{% endif %}{% endfor %}<span class="post-tags-inline"><a href="#{{ source }}" style="font-size: {% if count > 1 %}{{ count | times: 4 | plus: 105 | at_most: 180 }}{% else %}90{% endif %}%">{{ source | replace: " ", " " }}&nbsp;({{ count }})</a></span>{% else %} {% endif %}
{% endfor %}

---

<h2>Записи по авторам</h2>
{% for author in authors %}
  <h3 id="{{ author }}"><b>{{ author }}</b></h3>
  <ul>
  {% for post in site.posts %}
    {% if post.authors contains author %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
	{% endif %}
  {% endfor %}
  </ul>
{% endfor %}

---

<h2>Записи по источникам</h2>
{% for source in sources %}
  <h3 id="{{ source }}"><b>{{ source }}</b></h3>
  <ul>
  {% for post in site.posts %}
    {% if post.source contains source %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
	{% endif %}
  {% endfor %}
  </ul>
{% endfor %}