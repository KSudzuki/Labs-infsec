---
## Front matter
title: "Индивидуальный проект этап 3"
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

Установить hydra на kali linux

# Выполнение лабораторной работы

1. Установил последние обновления системы sudo командой - apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade

![](image/1.png){#fig:001 width=70%}

2. После обновления системы установил важные компоненты, необходимые для hydra

![](image/2.png){#fig:002 width=70%}

![](image/3.png){#fig:003 width=70%}

![](image/4.png){#fig:004 width=70%}

3. Клонировал репозиторий с Github

![](image/5.png){#fig:005 width=70%}

4. Зашёл в директорию thc-hydra и выполнил команду - ./configure

![](image/6.png){#fig:006 width=70%}

5. Выполнил команду с помощью sudo make и sudo make install

![](image/7.png){#fig:007 width=70%}

6. Проверил установилась ли hydra с помощью команды - hydra -help

![](image/8.png){#fig:008 width=70%}


# Выводы

Установил hydra на kali linux 