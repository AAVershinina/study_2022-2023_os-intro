---
## Front matter
title: "Индивидуальный проект "
subtitle: "Этап 2"
author: "Вершинина Ангелина Алексеевна"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Ознакомиться с файлами, которые помогут в создании и изменении сайта

# Задание

Добавить на сайт биографию и интересы. Написать посты

# Теоретическое введение


# Выполнение лабораторной работы

Размещу фотографию владельца сайта и добавлю краткое описание владельца(рис. @fig:001, @fig:002).

![Фото](image/1.png){#fig:001 width=70%}

![Описание](image/2.png){#fig:002 width=70%}

Добавлю информацию об интересах (рис. @fig:003)

![Интересы](image/3.png){#fig:003 width=70%}

Добавлю информацию об образовании (рис. @fig:004)

![Образование](image/4.png){#fig:004 width=70%}

Добавлю пост о прошедшей неделе (рис. @fig:005)

![Пост о прошедшей неделе](image/5.png){#fig:005 width=70%}

Добавлю пост о СI/CD (рис. @fig:006)

![Пост о СI/CD ](image/6.png){#fig:006 width=70%}

# Выводы

В результате выполнения работы я освоила навык добавления информации на сайт

# Список литературы{.unnumbered}

::: {#refs}
:::
