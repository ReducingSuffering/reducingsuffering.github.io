---
layout: blog
title: "Reducing Suffering: об уменьшении страданий на русском языке"
---
Проект посвящен уменьшению страданий во вселенной и различным смежным вопросам. Мы собираем, пишем, а также переводим англоязычные материалы.

Ниже находится [путеводитель](#contents) по всем нашим материалам. За новостями проекта можно следить в блоге [здесь](blog.html), а также в соцсетях <a href="https://vk.com/reducing_suffering">ВКонтакте</a> и <a href="https://t.me/reducing_suffering">Telegram</a>. Также вы можете воспользоваться [поиском](tags.html) по темам и авторам.

{% assign lists = site.lists | sort: "order" %}

<div class="contents" id="contents">
  <h2>Содержание</h2>
  <ul>
    {% for list in lists %}
    <li><a href="#{{ list.mark }}">{{ list.title }}</a>
      <ul>{% for sublist in list.sublists %}
        <li><a href="#{{ sublist.mark }}{{ sublist.url }}">{{ sublist.title }}</a>
		</li>
      {% endfor %}</ul>
	</li>{% endfor %}
  </ul>
</div>

{% for list in lists %}
  <h1 id="{{ list.mark }}">{{ list.title }} <a href="#contents" style="float: right">&#11181;</a></h1>
  <ul>{% for node in list.nodes %}
    <li class="sublist">{% include post-entry-by-id.html id=node %}</li>
  {% endfor %}
  {% for sublist in list.sublists %}
    <li><h2 id="{{ sublist.mark }}">{{ sublist.title }} <a href="#contents" style="float: right">&#11181;</a></h2>
    <ul>{% for node in sublist.nodes %}
      <li class="sublist">{% include post-entry-by-id.html id=node %}</li>
    {% endfor %}</ul></li>
  {% endfor %}
  </ul>
{% endfor %}