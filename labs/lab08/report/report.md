---
## Front matter
title: "Отчет по лабораторной работе № 8"
subtitle: "Дисциплина: архитектура компьютера"
author: "Выслоух Алиса Александровна"

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

Приобретение навыков написания программ с использованием циклов и обработкой аргументов командной строки.

# Задание

1. Реализация циклов в NASM

2. Обработка аргументов командной строки

3. Выполнение заданий для самостоятельной работы


# Выполнение лабораторной работы

## Реализация циклов в NASM

Создаю папку lab6 и перехожу в нее и создаю и создаю файл lab8-1.asm (рис. [-@fig:001]).

![Создание папки и файла.](image/1.png){#fig:001 width=70%}

В файл я ввела текст первой программы. (рис. [-@fig:002]).

![Ввод текста.](image/2.png){#fig:002 width=70%}

Создала исполняемый файл. (рис. [-@fig:003]).

![Создание исполняемого файла.](image/3.png){#fig:003 width=70%}

Я изменила текст программы, в теле цикла label добавила строку sub eax,1. Цикл закольцевался и стал бесконечным при вводе нечетных цифр и при вводе четных чисел он выводил нечетные на уменьшение (рис. [-@fig:004]).(рис. [-@fig:005]).

![Изменение файла при четных значениях.](image/4.png){#fig:004 width=70%}

![Изменение файла при нечетных значениях.](image/5.png){#fig:005 width=70%}

Я изменила текст программы так, чтобы цикл и счетчик работал правильно. По итогу после изменения программы, яисло проходки циклов стал соответствовать числу введенному с клавиатуры. (рис. [-@fig:006]). 

![Создание исполняемого файла после изменения.](image/6.png){#fig:006 width=70%}

Я создал файл lab8-2.asm и ввел туда программу, которая выводит все аргумент,которые ввели. Программа выводит все 3 аргумента которые ввели, но в разной вариации (рис. [-@fig:007]) (рис. [-@fig:007]).

![Создание исполняемого файла после изменения.](image/7.png){#fig:007 width=70%}

![Создание исполняемого файла после изменения.](image/8.png){#fig:008 width=70%}

Я создала файл lab8-3.asm. Ввел текст программы и запустил ее. Программа вывела сумму чисел, которые я ввела. (рис. [-@fig:009]) (рис. [-@fig:010]).

![Ввод текста программы.](image/9.png){#fig:009 width=70%}

![Запуск программы.](image/10.png){#fig:010 width=70%}

Я изменила программу, чтобы она выводила произведение введенных чисел. (рис. [-@fig:011]).

![ Ввод измененной программы.](image/11.png){#fig:011 width=70%}

Запуск измененной программы. (рис. [-@fig:012]).

![ Запуск изменной программы.](image/12.png){#fig:012 width=70%}

## Самостоятельная работа

Я написал программу, которая выводит сумму всех решений примера. Я получила 19 вариант. Введенные числа я придумала сама. (рис. [-@fig:011]).

![Создание и запуск файла.](image/13.png){#fig:013 width=70%}
![Создание и запуск файла.](image/14.png){#fig:014 width=70%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

