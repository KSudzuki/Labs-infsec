---
## Front matter
title: "Индивидуальный проект этап 5"
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

Научиться пользоваться Burp Suite

# Выполнение лабораторной работы

1. Запустил локальный веб-сервер (рис. [-@fig:001])

![](image/1.png){#fig:001 width=70%}

2. Запустил Burp Suite (рис. [-@fig:002])

![](image/2.png){#fig:002 width=70%}

3. Настроил прокси в браузере (рис. [-@fig:003])

![](image/3.png){#fig:003 width=70%}

4. Зашёл на сайт burp и скачал сертификаты (рис. [-@fig:004])

![](image/4.png){#fig:004 width=70%}

5. Установил сертификаты в браузер (рис. [-@fig:005])

![](image/5.png){#fig:005 width=70%}

6. Перезапустил BurpSuite и зашёл на наш сайт dvwa/login.php (рис. [-@fig:006])

![](image/6.png){#fig:006 width=70%}

7. Во вкладке Proxy отображаются запросы на вход (рис. [-@fig:007])

![](image/6.png){#fig:007 width=70%}

8. Во вкладке target мы можем посмотреть данные о цели (рис. [-@fig:008])

![](image/7.png){#fig:008 width=70%}

9. От туда мы можем отправить сайт во вкладку Intuder (рис. [-@fig:009])

![](image/8.png){#fig:009 width=70%}

10. Здесь мы можем заполнить данные, которые будут посылаться на сайт, и произвести атаку (рис. [-@fig:010])

![](image/9.png){#fig:010 width=70%}

11. Произведя атаку, мы можем посмотреть данные, в которых можно увидеть где мы оказываемся. При комбинации admin и password, мы оказываемся на index.php, что означает успешные переход на другую страницу - вход (рис. [-@fig:011])

![](image/10.png){#fig:011 width=70%}

12. Здесь мы можем заполнить данные, которые будут посылаться на сайт, и произвести атаку (рис. [-@fig:012])

![](image/9.png){#fig:012 width=70%}


# Выводы

Попробовали применить инструменты Burp Suite на практике, использовали наш локальный веб-сервер для проверки атаки и исследовали полученные данные.