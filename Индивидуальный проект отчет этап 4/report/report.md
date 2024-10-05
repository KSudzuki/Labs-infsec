---
## Front matter
title: "Индивидуальный проект этап 4"
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

Установить nikto и просканировать локальный веб-сервер

# Выполнение лабораторной работы

1. Установил nikto на kali linux (рис. [-@fig:001])

![](image/1.png){#fig:001 width=70%}

2. Проверил установилась ли nikto и её версию (рис. [-@fig:002])

![](image/2.png){#fig:002 width=70%}

3. Запустил локальный веб-сервер (рис. [-@fig:003])

![](image/3.png){#fig:003 width=70%}

4. Просканировал веб-сервер по полному URL (рис. [-@fig:004])

![](image/4.png){#fig:004 width=70%}

5. Просканировал веб-сервер по порту и ip-адресу (рис. [-@fig:005])

![](image/5.png){#fig:005 width=70%}

# Выводы

Установил nikto на kali linux.
Просканировал локальный веб-сервер с помощью nikto двумя способами.
При сканировании по полному URL, дается больше информации.