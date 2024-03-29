---
title: Что такое Git. Объясняем на схемах.
date: 2023-03-18
math: true
image:
  placement: 2
  caption: 'Image credit: [**John Moeses Bauan**](https://unsplash.com/photos/OGZtQF8iC0g)'
---

**Команды разработчиков пользуются системой контроля версий. Чаще всего это Git. Разбираемся, что это значит, зачем нужно и как устроено.**

## Git — это система коммитов

Представьте ситуацию: геймер доходит до финала, проигрывает и возвращается к началу уровня — попадает в ближайшую контрольную точку игры, где разработчики разрешили сохраниться. Если мы уберём контрольные точки, после каждого проигрыша придётся начинать игру заново.

*В программировании за сохранение кода в контрольных точках отвечает система контроля версий — специальная технология, которую можно подключить к любому проекту. Система контроля версий страхует от ошибок и возвращает код в то состояние, когда всё работало.*

Контрольные точки называются коммитами. Один коммит — это пакет изменений, хранящий информацию с добавленными, отредактированными или удалёнными файлами кода. В один коммит принято добавлять не более десяти изменений — так получается длинная история версий, которая позволяет в случае ошибки откатиться с минимальной потерей работоспособного кода.

[![схема 1](https://248006.selcdn.ru/main/upload/setka_images/14270913012021_e3ea06ecc4efe66fd609360c227a5daace25eda6.png.webp)](https://skillbox.ru/media/code/chto_takoe_git_obyasnyaem_na_skhemakh/)

## Git — это комплекс связанных веток

Коммиты располагаются на master-ветке — основной версии проекта, которая после завершения работы превратится в продукт.

*Система контроля версий позволяет создавать ответвления от master-ветки и экспериментировать с проектом, не мешая другим участника команды.*

Возьмём предыдущую схему, где мы обнаружили ошибку и откатились на один коммит назад. Чтобы поправить код, создадим несколько дополнительных веток и в каждой протестируем разные варианты решения проблемы. Когда решение найдено, ветку с правильным кодом переносим в master-ветку и сохраняем коммит. Лишние ветки оставляем или удаляем, поскольку они не влияют на проект и скрыты от других разработчиков — это ваш личный черновик.

[![схема 2](https://248006.selcdn.ru/main/upload/setka_images/14270913012021_db52642fc67f6c7c46657360f234a883af322464.png.webp)](https://skillbox.ru/media/code/chto_takoe_git_obyasnyaem_na_skhemakh/)

## Git — это распределённая система версий

Системы контроля версий бывают локальными, централизованными или распределёнными.

* Локальная система хранит файлы на одном устройстве, централизованная использует общий сервер, а распределённая — общее облачное хранилище и локальные устройства участников команды. В локальной системе удобно работать с большими проектами, но сложно взаимодействовать с удалённой командой.

* В централизованной системе налажена удалённая работа, но всё привязано к одному серверу. Любой сбой или взлом может повредить файлы проекта.

* В распределённой системе налажена удалённая работа. Если с файлами основного репозитория что-то случится — проект легко восстановить из копии любого участника команды.

*Из-за удобства и гибкости распределённая система версий Git считается современным форматом. Это стандарт для большинства ИТ-команд.*

[![схема 2](https://248006.selcdn.ru/main/upload/setka_images/14270913012021_27e9aa5bdf801f94f7728fe14d1ac08405e5a691.png.webp)](https://skillbox.ru/media/code/chto_takoe_git_obyasnyaem_na_skhemakh/)

## Зачем новичку учить Git

Git используется в большинстве компаний, где над проектом работает хотя бы два разработчика:

* Новый человек приходит в компанию и клонирует репозиторий проекта на ПК.

* Получает задачу, создаёт новую ветку и пишет код.

* Когда всё готово — отправляет запрос на добавление кода в master-ветку.

* Другие разработчики смотрят код, оставляют комментарии и указывают на ошибки.

* Новичок дорабатывает код, обновляет master-ветку и переходит к следующей задаче.

Это общая схема того, как проходит командная работа в проекте. В ней не учтены правила использования Git, которые каждая команда пишет под себя. Например, у каждой команды свой порядок проверки кода и свои критерии его готовности для добавления в master-ветку.

*Знание Git и знание правил использования Git в команде — это два разных навыка, которые можно сравнить с умением ездить на автомобиле и знанием правил дорожного движения. Если умеете управлять автомобилем — вам проще сконцентрироваться и быстро выучить правила. С Git аналогичная ситуация: если вы умеете управлять системой контроля версий, то можете сразу влиться в проект, не отвлекаться на второстепенные вещи и сосредоточиться на качестве кода.*


### Начинай развиваться и изучать Git уже сейчас!💪
