---
## Front matter
title: "Лабораторная работа №1"
subtitle: "Установка ОС Linux"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

Установка ОС на виртуальную машину и ее настройка.

# Теоретическое введение

Лабораторная работа подразумевает установку на виртуальную машину VirtualBox (https://www.virtualbox.org/) операционной системы Linux (дистрибутив Fedora).

# Выполнение лабораторной работы

Так как установка ОС на виртуальную машины была произведена в прошлом семестре, то буду пользоваться отчетом первой лабораторной работы первого семестра.

Первыми действиями были настройки виртуальной машины.(рис. [-@fig:0013], [-@fig:0014], [-@fig:0015], [-@fig:0016], [-@fig:0017], [-@fig:0018], [-@fig:0019], [-@fig:0020], [-@fig:0021])

![Настройка виртуальной машины](image/13.png){ #fig:0013 width=70% }

![Настройка виртуальной машины](image/14.png){ #fig:0014 width=70% }

![Настройка виртуальной машины](image/15.png){ #fig:0015 width=70% }

![Настройка виртуальной машины](image/16.png){ #fig:0016 width=70% }

![Настройка виртуальной машины](image/17.png){ #fig:0017 width=70% }

![Настройка виртуальной машины](image/18.png){ #fig:0018 width=70% }

![Настройка виртуальной машины](image/19.png){ #fig:0019 width=70% }

![Настройка виртуальной машины](image/20.png){ #fig:0020 width=70% }

![Настройка виртуальной машины](image/21.png){ #fig:0021 width=70% }

## Обновления

Необходимо обновить все пакеты (рис. [-@fig:001])

![Установка обновлений](image/1.png){ #fig:001 width=70% }

![Установка обновлений](image/2.png){ #fig:002 width=70% }

## Повышение комфорта работы

Необходимо установить программы для удобства работы в консоли (рис. [-@fig:003])

![Повышение комфорта работы](image/3.png){ #fig:003 width=70% }

## Автоматическое обновление

Установка программного обеспечения (рис. [-@fig:004])

![Установка программного обеспечения ](image/4.png){ #fig:004 width=70% }

Запуск таймера (рис. [-@fig:005])

![Запуск таймера](image/5.png){ #fig:005 width=70% }

## Отключение SELinux 

В данном курсе мы не будем рассматривать работу с системой безопасности SELinux.
Поэтому отключим его. (рис. [-@fig:006], [-@fig:007])

![Отключение SELinux](image/6.png){ #fig:006 width=70% }

![Отключение SELinux](image/7.png){ #fig:007 width=70% }

## Установка программного обеспечения для создания документации

Так как ранее были установлены Pandoc и TEXlive, то установлю расширения для удобства дальнейшей работы.(рис. [-@fig:008], [-@fig:009])

![Установка расширения](image/8.png){ #fig:008 width=70% }

![Установка расширения](image/9.png){ #fig:009 width=70% }

# Домашнее задание

**Задание**

Дождитесь загрузки графического окружения и откройте терминал. В окне терминала проанализируйте последовательность загрузки системы, выполнив команду dmesg.
(рис. [-@fig:0022])

![Последовательность загрузки системы](image/22.png){ #fig:0022 width=70% }

Можно использовать поиск с помощью grep

Получите следующую информацию. (рис. [-@fig:010], [-@fig:0011],[-@fig:0012])

1. Версия ядра Linux (Linux version).
2. Частота процессора (Detected Mhz processor).
3. Модель процессора (CPU0).
4. Объём доступной оперативной памяти (Memory available).
5. Тип обнаруженного гипервизора (Hypervisor detected).
6. Тип файловой системы корневого раздела.
7. Последовательность монтирования файловых систем.

![Задание](image/10.png){ #fig:0010 width=70% }

![Задание](image/11.png){ #fig:0011 width=70% }

![Задание](image/12.png){ #fig:0012 width=70% }


# Выводы

В результате выполнения данной лабораторной работы я систематизировала полученные ранее знания и обновила раннее установленную виртуальную машину.
