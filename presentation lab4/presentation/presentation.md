---
## Front matter
lang: ru-RU
title: Презентация к лабораторной работе №4 
subtitle: Дискреционное разграничение прав в Linux. Расширенные атрибуты
author:
  - Ким И. В. НФИбд-01-21
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---


# Цели и задачи

Получение практических навыков работы в консоли с расширенными атрибутами файлов
 
# Выполнение работы

## Зашел с двух консолей от имени пользователя guest и суперпользователя

![](image/1.png){#fig:001 width=70%}

## От имени пользователя guest определил расширенные атрибуты файла "file1"

![](image/2.png){#fig:002 width=70%}

## Установил права на файл "file1" разрешающие запись и чтение для владельца файла

![](image/3.png){#fig:003 width=70%}

## Попробовал установить на файл расширенный атрибут "a", получил отказ в доступе

![](image/4.png){#fig:004 width=70%}

## Установил на файл расширенный атрибут от имени суперпользователя

![](image/5.png){#fig:005 width=70%}

## От пользователя guest проверил правильность установленных атрибутов

![](image/6.png){#fig:006 width=70%}

## От имени пользователя guest попробовал выполнить запись, чтение, переименование и удаление файла "file1", получил отказ.

![](image/7.png){#fig:007 width=70%}

## Попробовал поменять права файла на "000" от обоих пользователей, получил отказ

![](image/8.png){#fig:008 width=70%}

![](image/9.png){#fig:009 width=70%}

## Снял расширенный атрибут "a" с файла, попробовал выполнить команды еще раз. Запись, чтение, переименование и удаление можно сделать. 

![](image/10.png){#fig:010 width=70%}

![](image/11.png){#fig:011 width=70%}

## Попробовал поменять права на "000", получил отказ.

## Повторил все действия с расширенным атрибутом "i". Запись, переименование и смена прав были запрещены, а чтение - разрешено.

![](image/12.png){#fig:012 width=70%}

![](image/13.png){#fig:013 width=70%}

## Составил таблицу прав действий с расширенными атрибутами "a" и "i".

![](image/14.png){#fig:014 width=70%}



## Выводы

Повысил свои навыки использование интерфейса командной строки, познакомился на примерах с тем, как используются основные и расширенные атрибуты
при разграничении доступа. Составил наглядные таблицы, поясняющие какие операции возможны при тех или иных установленных правах. Опрробовал 
действие на практике расширенных атрибутов "a" и "i".


