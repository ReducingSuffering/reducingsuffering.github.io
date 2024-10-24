---
layout: article
title: "Возможно ли согласование ИИ?"
authors:
  - Магнус Виндинг
translated_by: К. Кирдан
original: https://magnusvinding.com/2018/12/14/is-ai-alignment-possible/
original_date: "2018.12.14"
preview: https://magnusvinding.com/wp-content/uploads/2019/08/pexels-photo-247791.png?w=1400
---
<center><img src="https://magnusvinding.com/wp-content/uploads/2019/08/pexels-photo-247791.png?w=1400"/></center>

Задача согласования ИИ обычно огрубленно определяется как задача сделать так, чтобы мощный искусственный интеллект делал то, что мы — люди — хотим, чтобы он делал. Моя цель в этом эссе — объяснить, почему эта задача менее четко определена, чем, похоже, многие думают, и почему на деле ее невозможно «решить» с какой-либо точностью — не только на практике, но и вообще в принципе.

Обычно признаются две фундаментальные проблемы для согласования ИИ. Первая заключается в том, что есть более чем один вариант человеческих ценностей. В самом деле, во многих отношениях есть больше ценностных разногласий, чем люди склонны думать. Вторая проблема заключается в том, что даже если мы рассмотрим предпочтения одного человека, то, как я объясню, нет никакого способа воссоздать эти предпочтения в машине, чтобы она действовала так, как этот человек предпочел бы.

## Проблема 1. Не-единственность человеческих ценностей

Обычное представление о проблеме согласования ИИ сводится к следующему: у нас есть набор человеческих предпочтений, Х, которые мы должны каким-то образом (и это, как правило, считается очень трудной частью), сопоставить с целевой функцией У какой-нибудь машины, — скажем, через соответствие _f_, так, чтобы Х и У были в некотором смысле изоморфными. По крайней мере, так можно грубо охарактеризовать то, что люди пытаются сделать.

Говоря этими терминами, уделяется много больше внимания Y и _f_ по сравнению с X. Мой аргумент здесь состоит в том, что мы глубоко запутаны насчет природы X, и поэтому запутаны насчет согласования ИИ.

Первый момент путаницы касается ценностей человечества в целом. Обычно признается, что человеческие ценности нечеткие и что между людьми есть некоторые разногласия по поводу ценностей. Однако редко признается, насколько сильны эти разногласия на самом деле.

К примеру, разногласия касательно идеальной численности будущих популяций сентиентных существ почти тотальны, т. к. одни (напр., некоторые защитники так называемой [Асимметрии](https://en.wikipedia.org/wiki/Asymmetry_(population_ethics)) в демографической этике, а также антинаталисты, как Дэвид Бенатар) считают, что в идеале будущая популяция должна быть нулевой, тогда как другие, включая многих сторонников классического утилитаризма, считают, что будущая популяция должна в идеале быть очень большой. Можно привести много схожих примеров серьезных разногласий по самым фундаментальным и вытекающим из них этическим вопросам, в том числе по вопросу о том, может ли какое-либо позитивное благо [когда-либо перевесить](https://magnusvinding.com/2018/09/03/the-principle-of-sympathy-for-intense-suffering/) экстремальные страдания. И по многим из этих критичных разногласий найдется очень большое число людей по обе стороны.

Разные ответы на этические вопросы такого рода порождают не просто небольшие практические разногласия. Во многих случаях они подразумевают совершенно противоположные практические выводы. Дело не в нечеткости человеческих ценностей, а в их резкой, непримиримой противоречивости. И, следовательно, нет никакого способа отобразить совокупность человеческих предпочтений, Х, на единую, четко определенную целевую функцию так, чтобы это не вошло в _сильный_ конфликт с ценностями значительной части человечества. Это тривиальный момент, и все же большинство разговоров о согласовании ИИ с людьми, похоже, игнорируют этот факт.

## Проблема 2. Нынешние человеческие предпочтения не полностью определяют будущие действия

Вторая проблема и момент путаницы в отношении природы человеческих предпочтений заключается в том, что даже если мы сосредоточимся только на нынешних предпочтениях одного человека, то они фактически не будут и, по сути _не могут_, определить с большой точностью, какой мир этот человек предпочел бы создать в будущем.

Один из способов понять это — рассмотреть, сколько информации необходимо для того, чтобы представлять окружающий нас мир. Такое совершенно точное представление потребовало бы огромного объема информации, в действительности гораздо большего объема, чем может уместиться в нашем мозгу. Это так, даже если мы будем рассматривать только морально значимых существ вокруг нас — скажем, на этой планете. Их слишком много, чтобы мы могли иметь точное представление о них. Кроме того, их слишком много, чтобы мы могли иметь точные предпочтения насчет их индивидуальных состояний. Учитывая, что мы располагаем очень ограниченной информацией, все, что мы можем, это выразить крайне грубые и сжатые предпочтения относительно того, в каком состоянии должен находиться мир вокруг нас. Другими словами, предпочтения любого конкретного человека насчет точного идеального состояния мира в конкретный момент времени обречены быть крайне размытыми, и по всему миру в данный момент будут появляться моральные дилеммы, к которым предпочтения человека в их нынешнем состоянии не указывают единственного решения.

И это все только при рассмотрении нынешнего состояния мира. Когда мы рассмотрим будущие состояния, проблема определения идеальных состояний и решений до сих пор неизвестных моральных дилемм еще и взрывается в сложности, причем со временем взрывается экспоненциально. Это просто факт, и по сути вполне очевидный, что ни один мозг не может содержать достаточно информации для того, чтобы определить единственные или даже просто подходящие решения для всех моральных дилемм, которые возникнут в будущем. Так что же тогда может означать согласование ИИ даже с одним конкретным мозгом? Как мы можем определить Y в отношении этих будущих дилемм, если даже сама X не определяет их решений?

Мы, конечно, можем попытаться угадать, что мог бы сказать тот или иной человек, или мы сами, если бы столкнулся с определенной будущей моральной дилеммой, имея те или иные знания, но проблема в том, что наша экстраполированная догадка неизбежно будет просто весьма несовершенной догадкой. Ибо даже крошечное количество дополнительных знаний или опыта могут легко изменить представление человека о данной моральной дилемме на противоположное тому, что было до того (например, сам я перешел от классического утилитаризма к негативному, основываясь на скромном количестве информации в виде [аргументов](https://magnusvinding.com/2018/09/03/suffering-focused-ethics/), которые я до этого не рассматривал). Эта высокая чувствительность к небольшим изменениям в нашем мозге подразумевает, что даже система с почти совершенной информацией о текущем состоянии мозга какого-нибудь человека будет вынуждена делать очень неуверенное предположение о том, что этот человек на деле предпочел бы в той или иной моральной дилемме. И чем дальше мы продвигаемся вперед, отдаляясь от знакомых нам обстоятельств и контекста, тем выше будет неуверенность.

По аналогии рассмотрим задачу согласования ИИ с нашими предками, жившими десять миллионов лет назад. Каковы были бы их предпочтения в отношении, скажем, будущей космической колонизации? Можно возразить, что они недостаточно определенные из-за того, что наши предки не могли представить себе такую возможность. Но то же самое относится и к нам в случае вещей, которые мы не можем сейчас постичь, таким как чуждые нам состояния сознания. Наши нынешние предпочтения говорят столь же мало об (отрицательной или положительной) ценности таких состояний, как предпочтения наших предков десять миллионов лет назад говорили о космической колонизации.

Более ощутимой аналогией может служить следующее. Насколько мы уверены в том, что, основываясь на знании о текущем состоянии вашего мозга, мы можем определить ваши пищевые предпочтения на двадцать лет в будущее в отношении блюд, изготовленных из ингредиентов, которые еще не изобретены? Эти предпочтения, видимо, будут зависеть от контингентных факторов окружающей среды, разделяющих тогда и сейчас. Можно смело сказать, что уверенность невелика. И это относится не только к пищевым предпочтениям, но и к самым важным вопросам. Наши нынешние предпочтения не могут реалистично определить с какой-либо значительной точностью то, что мы считали бы идеальным в пока еще неизвестных реалистичных сценариях будущего. Таким образом, в более общем плане, не может быть такой вещи, как экстраполяция или сохранение ценностей в каком-либо нерасплывчатом смысле. Ни в одном человеческом уме никогда не содержался и никогда не мог бы содержаться набор предпочтений, которые оценивали бы на порядки больше, чем лишь самый крошечный кусочек (сильно сжатых версий) реальных состояний и вариантов выбора, с которыми агент в нашем мире, вероятно, в будущем столкнется. Думать иначе было бы странной платонизацией человеческих предпочтений. Мы просто не располагаем достаточной информацией в наших головах, чтобы у нас были такие детализированные ценности.

Правда в том, что наши предпочтения — это не какая-то фиксированная сущность, которая однозначно определяет будущие действия; они просто не могут быть таковыми. Скорее, наши предпочтения сами по себе интерактивны и адаптивны по своей природе, они изменяются в ответ на новый опыт и новую информацию, с которой мы сталкиваемся. Таким образом, сказать, что мы можем «идеализировать» наши нынешние предпочтения, с тем чтобы получить ответы на все реалистичные будущие моральные дилеммы, — все равно, что назвать эволюцию ДНК наших предков по направлению к ДНК человека «идеализацией ДНК». В обоих случаях мы не находим никаких скрытых Глубоких Сущностей, ожидающих очищения; никакой информации, указывающей на лишь одно конкретное решение всех реалистичных будущих «проблем». Все, что мы находим — это физические системы, которые развиваются контингентно на основе получаемых ими данных[^1].

Суть всего этого не в том, что нет смысла выделять ресурсы на обеспечение безопасности будущих машин. Мы по-прежнему можем осмысленно и кооперативно стремиться к внедрению в наши машины и институты таких правил и механизмов, которые кажутся оптимальными в математическом ожидании с точки зрения наших соответствующих огрубленных ценностей. Вывод здесь состоит в том, что: 1) созданные правила не могут быть результатом универсально разделяемой человеческой воли или чего-то подобного; самое близкое, что возможно, — это правила, воплощающие какой-то компромисс между людьми с сильно расходящимися ценностями; и 2) такое воплощение огрубленных правил на деле составляет верхнюю границу того, чего мы можем ожидать добиться в этом отношении. В самом деле, это все, чего мы можем ожидать насчет влияния на будущее в целом: влияние будет грубым и неточным, управление будет ограничено той информацией, которой мы можем обладать и которую можем передать. Идея машины, которая будет делать именно то, чего мы хотим, и чье устройство, следовательно, было бы рычагом для точного контроля над будущим, — это несбыточная мечта.

---

[^1]: Обратите внимание, что такой взгляд на наши предпочтения не противоречит ценностному или моральному реализму. По аналогии, рассмотрим человеческие предпочтения и поиск истины: люди способны открыть многие истины о вселенной, но большинство из этих истин не скрыты в нашей ДНК или наших предпочтениях и не экстраполируются из них. Действительно, во многих случаях мы лишь обнаруживаем эти истины, активно преодолевая, а не «экстраполируя» наши непосредственные предпочтения (предпочтения иметь комфортные и интуитивные убеждения, скажем). То же самое можно сказать и о ценностях и морали.