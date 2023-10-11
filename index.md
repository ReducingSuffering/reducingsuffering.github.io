---
layout: blog
title: "Reducing Suffering"
nav_id: 0
---
**(Это тестовая версия сайта!)**

Проект посвящен уменьшению страданий во вселенной и различным смежным вопросам: от (мета)этики до астробиологии и безопасности искусственного интеллекта. Мы пишем, собираем, а также переводим англоязычные материалы.

Ниже находится путеводитель по всем нашим материалам. Также для поиска вы можете воспользоваться [блогом](blog.html) и [тегами](tags.html). За новостями проекта можно следить в соцсетях <a href="https://vk.com/reducing_suffering">ВКонтакте</a> и <a href="https://t.me/reducing_suffering">Telegram</a>.

<div class="contents">
  <h2>Содержание</h2>
  <ul>
    {% for list in site.lists %}
    <li><a href="#{{ list.mark }}">{{ list.title }}</a>
      <ul class="ulcirc">{% for sublist in list.sublists %}
        <li><a href="#{{ sublist.mark }}{{ sublist.url }}">{{ sublist.title }}</a>
          <ul class="ulcirc">{% for subsublist in sublist.sublists %}
            <li><a href="#{{ subsublist.mark }}{{ subsublist.url }}">{{ subsublist.title }}</a></li>
          {% endfor %}</ul>
		</li>
      {% endfor %}</ul>
	</li>{% endfor %}
  </ul>
</div>

---

{% for list in site.lists %}
  <h1 id="{{ list.mark }}">{{ list.title }}</h1>
  <ul>{% for node in list.nodes %}
    <li>{% include post-entry-by-id.html id=node %}</li>
  {% endfor %}
  
  {% for sublist in list.sublists %}
    <li>{% if sublist.url %}<h2><a href="#{{ sublist.url }}">{{ sublist.title }}</a></h2>{% else %}<h2 id="{{ sublist.mark }}">{{ sublist.title }}</h2>{% endif %}
    <ul>{% for node in sublist.nodes %}
      <li>{% include post-entry-by-id.html id=node %}</li>
    {% endfor %}
	
	{% for subsublist in sublist.sublists %}
      <li><h3 id="{{ subsublist.mark }}">{{ subsublist.title }}</h3>
      <ul>{% for node in subsublist.nodes %}
        <li>{% include post-entry-by-id.html id=node %}</li>
      {% endfor %}</ul></li>
    {% endfor %}
	
	</ul></li>
  {% endfor %}
  
  </ul>
{% endfor %}

---

[Все в обратном хронологическом порядке](blog.html)<br>
[Поиск по темам](tags.html)