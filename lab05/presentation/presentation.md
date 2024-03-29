---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
author: |
	Роман В. Иванов - студент группы НКНбд-01-18
date: 13.11.2021

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов

## Прагматика выполнения

- Помимо прав администратора в некоторых случаях требуются средства разработки приложений. Для разграничения их прав нужно использовать дополнительные атрибуты.

## Цель выполнения лабораторной работы

- Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

## Задачи выолнения работы

- Подготовить лабораторный стенд
- Рассмотреть компиляцию программ
- Создать программы
- Исследовать Sticky-бит

## Результаты выполнения лабораторной работы

- Подготовил лабораторный стенд (рис - @fig:001).

![Установка компилятора gcc](image/1.png){ #fig:001 width=70% }

##

- Рассмотрел комплияцию программ (рис -@fig:002).

![Проверка названий компиляторов](image/3.png){ #fig:003 width=70% }

##

- Провел работу с программами (рис -@fig:003, рис -@fig:004, рис -@fig:005).

![Смена владельца и атрибутов от имени суперпользователя](image/10.png){ #fig:003 width=70% }

##

![Создание программы \texttt{readfile.c}](image/15_2.png){ #fig:004 width=70% }

##

![Проверка чтения файла](image/21.png){ #fig:005 width=70% }

##

- Исследовал Sticky-бит (рис -@fig:006, рис -@fig:007, рис -@fig:008).

![Создание файла и внесение записи в него](image/24.png){ #fig:006 width=70% }

##

![Попытка удаления файла от имени пользователя \texttt{guest2}](image/31.png){ #fig:007 width=70% }

##

![Проведение различных операций после удаления атрибута \texttt{t}](image/36.png){ #fig:008 width=70% }

##

Таким образом, я изучил механизмы изменения идентификаторов, применения SetUID- и Sticky-битов. Получил практические навыки работы в консоли с дополнительными атрибутами. Рассмотрел работу механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.