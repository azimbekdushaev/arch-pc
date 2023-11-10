---
## Front matter
title: "Отчёт по лабораторной работе 5"
subtitle: "Архитектура компьютера"
author: "Душаев Азимбек Юсуфович НКАбд-02-23"

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

Целью работы является приобретение практических навыков работы в Midnight Commander. 
Освоение инструкций языка ассемблера mov и int.

# Выполнение лабораторной работы

1. Открыл Midnight Commander и перешел в каталог ~/work/arch-pc. Создал каталог lab05.

![Создание каталога](image/01.png){ #fig:001 width=70%, height=70% }

2. В каталоге lab05 создал файл lab05-1.asm. Открыл файл для редактирования и написал соответствующий код.

![Программа lab05-1.asm](image/02.png){ #fig:002 width=70%, height=70% }

3. Открыл файл lab05-1.asm для просмотра и проверил написанный код.

![Просмотр файла lab05-1.asm](image/03.png){ #fig:003 width=70%, height=70% }

4. Скомпилировал файл lab05-1.asm и получил исполняемый файл. Проверил, как работает полученный исполняемый файл.

![Запуск программы lab05-1.asm](image/04.png){ #fig:004 width=70%, height=70% }

5. Скачал файл in_out.asm и добавил его в рабочий каталог. Скопировал содержимое lab05-1.asm в новый файл lab05-2.asm.

![Копирование файла](image/05.png){ #fig:005 width=70%, height=70% }

6. В файле lab05-2.asm написал код программы. Скомпилировал программу и проверил ее запуск.

![Программа lab05-2.asm](image/06.png){ #fig:006 width=70%, height=70% }

![Запуск программы lab05-2.asm](image/07.png){ #fig:007 width=70%, height=70% }

7. В файле lab05-2.asm заменил вызов подпрограммы sprintLF на sprint, чтобы вывод строки происходил без перехода на следующую строку. 
Пересобрал исполняемый файл.

![Программа lab05-2.asm](image/08.png){ #fig:008 width=70%, height=70% }

![Запуск программы lab05-2.asm](image/09.png){ #fig:009 width=70%, height=70% }

8. Скопировал программу lab05-1.asm и изменил код, чтобы программа выводила приглашение типа "Введите строку:", затем считывала строку с клавиатуры и выводила введенную строку на экран.

![Программа lab05-3.asm](image/10.png){ #fig:010 width=70%, height=70% }

![Запуск программы lab05-3.asm](image/11.png){ #fig:011 width=70%, height=70% }

9. Скопировал программу lab05-2.asm и сделал аналогичные изменения, но теперь использовал возможности из файла in_out.asm для ввода-вывода строк.

![Программа lab05-4.asm](image/12.png){ #fig:012 width=70%, height=70% }

![Запуск программы lab05-4.asm](image/13.png){ #fig:013 width=70%, height=70% }

# Выводы

Научились писать базовые ассемблерные программы. Освоили ассемблерные инструкции mov и int.
