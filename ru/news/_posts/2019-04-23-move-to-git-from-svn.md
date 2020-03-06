---
layout: news_post
title: "Репозиторий Ruby переходит с Subversion на Git"
author: "hsbt"
translator: "shprotru"
date: 2019-04-23 00:00:00 +0000
lang: ru
---

Сегодня канонический репозиторий языка программирования Ruby переведен из Subversion в Git.

Веб-интерфейс нового репозитория [https://git.ruby-lang.org](https://git.ruby-lang.org), реализован на базе cgit. Мы можем сохранять хэши коммитов участников напрямую в репозиторий Ruby.

## Политики разработки

* Не используем главную ветку в cgit.
* Репозиторий GitHub останется лишь зеркалом. Не пользуемся "Merge pull request".
* Ветки ruby_2_4, ruby_2_5, и ruby_2_6 будут продолжены разрабатываться на SVN. Не вносим никаких изменений на cgit.
* Начиная с ruby_2_7, пользуемся cgit для разработки стабильных веток.
* Не пользуемся слияниями коммитов.

## Отдельные благодарности

* k0kubun

  k0kubun в агрессивной манере запилил инструменты для релизов и портирования рабочих процессов, а также обновил хук-скрипт для git.

* naruse

  naruse обновил список новшеств для Ruby CI и Redmine (bugs.ruby-lang.org).

* mame

  mame прикрутил скрипт для уведомлений о коммитах в slack.

## Предстоящие работы

Нам всё ещё нужно закончить некоторые задачи. Если вы обнаружите проблемы связанные с миграцией на Git, пожалуйста, дайте нам знать [https://bugs.ruby-lang.org/issues/14632](https://bugs.ruby-lang.org/issues/14632).

Наслаждайтесь!