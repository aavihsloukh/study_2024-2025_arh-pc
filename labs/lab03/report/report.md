---
## Front matter
title: "Отчет по лабораорной работе"
subtitle: "Дисциплина: архтектура компьютеров"
author: " Выслоух Алиса Александровна"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Задание
 1.  заполнение отчета по лабораторной работе №3 с помощью языка размеки markdown.
 2. Задание для самостоятельной работы.
 

# Выполнение лабораторной работы

Открываю терминал, перехржу в каталог курса из прошлой лабораторной работы и и ввожу команду gitpull, тем самым обновляя локальный репозиторий, скачав изменения. (рис. [-@fig:001])
![Команда gitpull. Перемещение между дерикториями. ](pic1.png){#fig:001 width=70%}

Перехожу в каталог с шаблоном отчета по лабораторной работе №3.(рис. [-@fig:002])
![Перемещение между директорияи.](pic2.png){#fig:002 width=70%}

Провожу компиляцию щаблона с использованием Makefile. (рис. [-@fig:003])
![Компиляция шаблона.](pic3.png){#fig:003 width=70%}

Проверяю успешность создания файла pdf. (рис. [-@fig:004])
![Проверка pdf.](pic5.png){#fig:004 width=70%}

Проверяю успешность создания файла docx. (рис. [-@fig:005])
![Проверка docx.](pic.png){#fig:005 width=70%}

Удаляю  полученные файлы с использованием команды make clean. (рис. [-@fig:006])
![Удаление файлов.](pic.png){#fig:006 width=70%}

Проверяю, что файлы удалены. (рис. [-@fig:007])
![Проверка удаления.](зз.png){#fig:007 width=70%}

Открываю файл report.md с помощью текстового редактора gedit. (рис. [-@fig:008])
![Открытие файла.](pic7.png){#fig:008 width=70%}

Заполняю отчет с помощью языка разметки markdown. (рис. [-@fig:009])
![Заполнение работы.](pic8.png){#fig:009 width=70%}

 Комплимирую файл с отчетом. Загружаю отчет на github. 


Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001]).

![Название рисунка](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
