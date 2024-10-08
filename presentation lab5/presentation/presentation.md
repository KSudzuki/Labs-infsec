---
## Front matter
lang: ru-RU
title: Презентация к лабораторной работе №5 
subtitle: Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов
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

Изучение механизмов изменения идентификаторов, применения
SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма
смены идентификатора процессов пользователей, а также влияние бита
Sticky на запись и удаление файлов

# Выполнение лабораторной работы

# Создание программы

## Создал программу simpleid.c 

![](image/1.png){#fig:001 width=70%}

## Записал код программы в simpleid.c 

![](image/2.png){#fig:002 width=70%}

## Скомпилировал и выполнил программу simpleid.c 

![](image/3.png){#fig:003 width=70%}

## Изменил код программы в simpleid.c 

![](image/4.png){#fig:004 width=70%}

## Скомпилировал и выполнил программу simpleid2.c 

![](image/5.png){#fig:005 width=70%}

## От имени суперпользователя поменял права на файл simpleid2.c, поменял владельца файла и выполнил программу 

![](image/6.png){#fig:006 width=70%}

 - Результаты выполнения отличаются.

## Создал файл readfile.c 

![](image/7.png){#fig:007 width=70%}
 
## Записал код программы в readfile.c 

![](image/8.png){#fig:008 width=70%}

## Скомпилировал readfile.c 

![](image/9.png){#fig:009 width=70%}

## Сменил права и владельца readfile.c, попрбовал от имени пользователя guest прочитать файл, получил отказ 

![](image/10.png){#fig:010 width=70%}

## С помощью программы readfile прочитал файл /etc/shadow 

![](image/11.png){#fig:011 width=70%}

# Исследование Sticky-бита

## Проверил установлен ли атрибут Sticky на директории /tmp , создал в ней файл file91.txt

![](image/12.png){#fig:012 width=70%}

## Проверил атрибуты у файла file01.txt , поменял атрибуты на чтение и запись для остальных пользователей 

![](image/13.png){#fig:013 width=70%}

## От пользователя guest 2 попробовал прочитать, изменить и удалить file01.txt, получилось только прочитать   

![](image/14.png){#fig:014 width=70%}

## От имени суперпользователя снял атрибут t у /tmp 

![](image/15.png){#fig:015 width=70%}

## От имени guest 2 проверил, что у директории /tmp нет атрибута t. Попробовал сделать команды еще раз, ничего не поменялось. 

![](image/16.png){#fig:016 width=70%}

## Поменял права файла file01.txt на 666 

![](image/17.png){#fig:017 width=70%}

## Попробовал выполнить команды еще раз, получилось сделать все, кроме удаления

![](image/18.png){#fig:018 width=70%}

## Удалил атрибут t и выполнил команды, получилось выполнить все, включая удаление 

![](image/19.png){#fig:019 width=70%}

# Выводы

Изучил механизм изменения идентификаторов, применяя SetUID и Sticky-битов. Получил практические навыки работы в консоли с дополнительными атрибутами. Рассмотрел работу механизма смены идентификатора процессов пользователей, а также влияния бита Sticky на запись и удаление файлов.


