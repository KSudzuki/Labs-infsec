---
## Front matter
title: "Индивидуальный проект этап 2"
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

- Научиться основным способам тестирования веб приложений

- Установить и настроить DVWA на Kali linux

# Выполнение лабораторной работы

1. Клонировал DVWA с https://github.com/digininja/DVWA

![](image/1.png)


2. Переименовал директорию DVWA на dvwa

![](image/2.png)

3. Задал права пользователя для директории

![](image/3.png)

4. Зашел в директорию dvwa/config

![](image/4.png)

5. Проверил что в ней есть 

![](image/5.png)

6. Открыл файл config.inc.php

![](image/6.png)

7. Файл config.inc.php

![](image/7.png)

8. Заменил в нем db_user и db_password на user и pass

![](image/8.png)

9. Посмотрел мой mysql-server

![](image/9.png)

10. Установил mysql-server 

![](image/10.png)

11. Запустил mysql

![](image/11.png)

12. Посмотрел статус mysql

![](image/12.png)
![](image/13.png)

13. Зашел в mysql

![](image/14.png)

14. Создал пользователя и дал ему все права

![](image/15.png)

15. Зашёл в папку /etc/php/8.2/apache2

![](image/16.png)

16. Посмотрел что в ней есть и открыл файл php.ini

![](image/17.png)

17. Файл php.ini

![](image/18.png)

18. Нашел в нем allow_url_fopen и allow_url_include и поменял на "On"

![](image/19.png)

19. Запустил apache2 и проверил его статус

![](image/20.png)

20. Зашёл на Localhost 127.0.0.1/dvwa/setup.php

![](image/21.png)

21. Ввёл логин и пароль admin password

![](image/22.png)

22. Поменял защиту на low

![](image/23.png)

# Выводы

- Установил и настроил DVWA на Kali linux