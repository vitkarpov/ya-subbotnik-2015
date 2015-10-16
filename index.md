---

layout: default

style: |

    .images.row img {
      width: 300px;
    }

---

# Яндекс

## **{{ site.presentation.title }}** {#cover}

<div class="s">
    <div class="service">{{ site.presentation.service }}</div>
</div>

{% if site.presentation.nda %}
<div class="nda"></div>
{% endif %}

<div class="info">
	<p class="author"><a href="{{ site.author.link }}">{{ site.author.name }}</a>, <br/> {{ site.author.position }}</p>
    <p class="author">#yasubbotnik, Москва, 17 октября 2015 года</p>
</div>

## ![](pictures/disk.png)
{:.cover .w}

## ![](pictures/disk-mini.png)
{:.cover .w}

## **Задача и метрики**

## ![](pictures/waterfall.jpg)
{:.cover .w}

## ![](pictures/agile.jpg)
{:.cover .w}

## Задачи

* привлечение новых пользователей
* вход в свой Диск

## Метрика

* CTR кнопок «Завести Диск» и «зарегистрироваться» в форме логина

## Простой эксперимент

    <% if experiment %>
        <video poster="<%= preview %>">
            <source src="<%= video %>" />
        </video>
    <% else %>
        <img src = "<%= preview %>" />
    <% endif %>

## **Что нужно учитывать**

## Однородность контрольной выборки

* Показываем один и тот же вариант каждой группе пользователей
* ...Не показываем видео, если не смогли загрузить в течении 2 секунд (считаем канал слабым)
* ...Не показываем видео на мобильных (считаем канал слабым)

## Время проведения эксперимента

* Нужно подождать пока приборы «успокоятся»
* ...В нашем случае, проводили эксперимент в течении **1 месяца**

## Результаты

> CTR кнопки «Завести свой Диск»

| Видео | on       | off      |
+-------|----------|----------|
| CTR   | **7.04%**| **7.86%**|
+-------|----------|----------+

> CTR кнопки «зарегистрироваться»

| Видео | on       | off      |
+-------|----------|----------|
| CTR   | 1.75%    | **1.98%**|
+-------|----------|----------+

## Более сложный эксперимент
{:.images .row}

![](pictures/disk-mini.png)

![](pictures/disk-middle.png)

![](pictures/disk.png)

## ![](pictures/plot1.jpg)
{:.cover .h}

## ![](pictures/plot2.jpg)
{:.cover .h}

## ![](pictures/plot3.jpg)
{:.cover .h}

## Выводы

* Четко сформулировать цель и определить метрики
* ...Проводить эксперименты для проверки своих гипотез

## **Контакты** {#contacts}

<div class="info">
    <p class="author">{{ site.author.name }}</p>
    <p class="position">{{ site.author.position }}</p>

    <div class="contacts">
        <p class="contacts-left mail">vitkarpov@yandex-team.ru</p>
        <!-- <p class="contacts-right contacts-top twitter">@twitter</p> -->
        <!-- <p class="contacts-right vk">vitkarpov</p> -->
        <p class="contacts-right facebook">vitkarpov</p>
    </div>
</div>
