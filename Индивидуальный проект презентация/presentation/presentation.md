---
## Front matter
lang: ru-RU
title: Индивидуальный проект этап 2
subtitle: Информационная безопасность
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

## Цели и задачи

- Научиться основным способам тестирования веб приложений

- Установить и настроить DVWA на Kali linux

## Выполнение работы

1. Клонировал DVWA с https://github.com/digininja/DVWA 

![](image/1.png)

## Выполнение работы

2. Переименовал директорию DVWA на dvwa

![](image/2.png)

## Выполнение работы

3. Задал права пользователя для директории

![](image/3.png)

## Выполнение работы

4. Зашел в директорию dvwa/config

![](image/4.png)

## Выполнение работы

5. Проверил что в ней есть 

![](image/5.png)

## Выполнение работы

6. Открыл файл config.inc.php

![](image/6.png)

## Выполнение работы

7. Файл config.inc.php

![](image/7.png)

## Выполнение работы

8. Заменил в нем db_user и db_password на user и pass

![](image/8.png)

## Выполнение работы

9. Посмотрел мой mysql-server

![](image/9.png)

## Выполнение работы

10. Установил mysql-server 

![](image/10.png)

## Выполнение работы

11. Запустил mysql

![](image/11.png)

## Выполнение работы

12. Посмотрел статус mysql

![](image/12.png)
![](image/13.png)

## Выполнение работы

13. Зашел в mysql

![](image/14.png)

## Выполнение работы

14. Создал пользователя и дал ему все права

![](image/15.png)

## Выполнение работы

15. Зашёл в папку /etc/php/8.2/apache2

![](image/16.png)

## Выполнение работы

16. Посмотрел что в ней есть и открыл файл php.ini

![](image/17.png)

## Выполнение работы

17. Файл php.ini

![](image/18.png)

## Выполнение работы

18. Нашел в нем allow_url_fopen и allow_url_include и поменял на "On"

![](image/19.png)

## Выполнение работы

19. Запустил apache2 и проверил его статус

![](image/20.png)

## Выполнение работы

20. Зашёл на Localhost 127.0.0.1/dvwa/setup.php

![](image/21.png)

## Выполнение работы

21. Ввёл логин и пароль admin password

![](image/22.png)

## Выполнение работы

22. Поменял защиту на low

![](image/23.png)

## Выводы

- Установил и настроил DVWA на Kali linux