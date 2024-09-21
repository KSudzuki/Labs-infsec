---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Информационная безопасность"
author: "Ким Илья Владиславович НФИбд-01-21"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

- Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей

## Выполнение лабораторной работы

1. Добавил гостевую учетную запись guest2 и задал пароль | useradd guest | passwd guest

![](image/1.png)

2. Добавил пользователя guest2 в группу guest | gpasswd -a guest2 guest

![](image/2.png)

3. Осуществил вход от двух пользователей ( guest и guest2 ) на двух разных консолях 

![](image/3.png)

4. От имени пользователя guest2 выполнил регистрацию пользователя guest2 в группe guest | newgrp guest

![](image/4.png)

5. От имени пользователя guest изменил права директории /home/guest, разрешив все действия для пользователей группы | chmod g+rwx /home/guest

![](image/5.png)

6. От имени пользователя guest снял с директории /home/guest/dir1 все атрибуты | chmod 000 dirl

![](image/6.png)

7. Меняя атрибуты директории и файла от имени пользователя guest, заполнил таблицу прав доступа и минимальных прав доступа

![](image/7.png)
![](image/8.png)

![](image/9.png)

# Выводы

- Полученил практические навыки работы в консоли с атрибутами файлов для групп пользователей