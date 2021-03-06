---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе №4"
subtitle: "Дисциплина: Операционные системы"
author: "Аветисян Давид Артурович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться с операционной системой Linux, получить практические навыки работы с консолью и некоторыми графическими менеджерами рабочих столов операционной системы.

# Задание

1. Ознакомиться с теоретическим материалом.
2. Загрузить компьютер.
3. Перейти на текстовую консоль. Сколько текстовых консолей доступно на вашем компьютере?
4. Перемещаться между текстовыми консолями. Какие комбинации клавиш необходимо при этом нажимать?
5. Зарегистрироваться в текстовой консоли операционной системы. Какой логин вы при этом использовали? Какие символы отображаются при вводе пароля?
6. Завершить консольный сеанс. Какую команду или комбинацию клавиш необходимо для этого использовать?
7. Переключиться на графический интерфейс. Какую комбинацию клавиш для этого необходимо нажать?
8. Ознакомиться с менеджером рабочих столов. Как называется менеджер, запускаемый по умолчанию?
9. Поочерёдно зарегистрироваться в разных графических менеджерах рабочих столов (GNOME, KDE, XFCE) и оконных менеджерах (Openbox). Продемонстрировать разницу между ними, сделав снимки экрана (скриншоты). Какие графические менеджеры установлены на вашем компьютере?
10. Изучить список установленных программ. Обратить внимание на предпочтительные программы для разных применений. Запустите поочерёдно браузер, текстовой редактор, текстовой процессор, эмулятор консоли. Укажите названия программ.


# Выполнение лабораторной работы

1. Ознакомился с теоретическим материалом, представленном в лабораторной работе №4 на ТУИСе (рис. -@fig:001).

![Ознакомление с теоретическим материалом](image04/img01.png){ #fig:001  }

2. Загрузил компьютер.

3. Перешёл на текстовую консоль. На моём компьютере доступно 6 текстовых консолей. Скриншот в текстовой консоле сделать нельзя, поэтому все последующие шаги буду описывать в отчёте. Для переключения из графического режима в одну из текстовых виртуальных консолей достаточно нажать комбинацию клавиш "Ctrl+Alt+Fn", где n — номер необходимой виртуальной консоли.

4. Научился перемещаться между текстовыми консолями. Переключение между консолями осуществляется при помощи сочетания клавиши "Ctrl+Alt" с одной из функциональных клавиш (F1–F6). 

5. Зарегистрировался в текстовой консоли операционной системы. При регистрации я использую логин и пароль от учётной записи операционной системы. При вводе логина все символы отображаются полностью, а вот при вводе пароля символы не отображаются. Процедура регистрации в графическом режиме аналогична регистрации в текстовом режиме.

6. Завершил консольный сеанс. Для того, чтобы завершить сеанс в текстовой консоли необходимо испоьзовать комбинацию клавиш "Ctrl+D" или ввести команду logout.

7. Переключился на графический интерфейс. Для перехода из текстового режима в графический интерфейс необходимо нажать комбинацию клавиш "Ctrl+Alt+F7". 

8. Ознакомился с менеджером графических столов. Менеджер, запускаемый по умолчанию - Ubuntu (рис. -@fig:002).

![Графический менеджер Ubuntu](image04/img02.png){ #fig:002 }

9. Поочерёдно зарегистрировался в разных графических менеджерах рабочих столов: GNOME, KDE, XFCE (рис. -@fig:003) (рис. -@fig:004). Разница между графическими менеджерами продемонстрирована на скриншотах.  Так же зарегистрировалась в оконном менеджере Openbox. В данном оконном менеджере нельзя сделать скриншот (разница с остальными графическими менеджерами состоит в том, что в самом начале сеанса открывается "Чёрный экран"). На моём компьютере установлены следующие графические менеджеры: 
- GNOME;
- GNOME на Xorg;
- Openbox;
- Ubuntu;
- Plasma;
- Plasma (Wayland);
- Сеанс.
- Сеанс Xfce.

![Графический менеджер GNOME](image04/img03.png){ #fig:003 }

![Графический менеджер KDE](image04/img04.png){ #fig:004 }

10. Изучил список установленных программ. Обратил внимание на предпочтительные программы для разных применений. Запустил браузер (рис. -@fig:005), текстовый редактор (рис. -@fig:006), текстовый процессор (рис. -@fig:007), эмулятор консоли (рис. -@fig:008). Название программ:
- для браузеpа - Mozila Firefox;
- для текстового редактора - Блокнот;
- для текстового процессора -  LibreOffice Writer;
- эмулятор консоли - Konsole.

![Браузер - Mozila Firefox](image04/img05.png){ #fig:005 }

![Текстовый редактор - Блокнот](image04/img06.png){ #fig:006  }

![Текстовый процессор - LibreOffice Writer](image04/img07.png){ #fig:007 }

![Эмулятор консоли - Konsole](image04/img08.png){ #fig:008 }

# Контрольные вопросы

1. Компьютерный терминал — устройство ввода–вывода, основные функции которого заключаются в вводе и отображении данных.
У компьютерного терминала есть преимущества перед графическим интерфейсом:
- снижение начальных затрат на приобретение персональных компьютеров, поскольку требования к их конфигурации минимальны, а тонкие клиенты производятся без встроенных носителей информации.
- унификация – все терминалы имеют одинаковый набор программного обеспечения.
- простота первоначального внедрения – нет необходимости настраивать каждый персональный компьютер в отдельности, присутствует централизованное управление информационным процессом.
- экономия времени системного администратора. Все тонкие клиенты абсолютно одинаковы, вероятность поломок сведена к минимуму, а программное обеспечение установлено только на сервере.
- масштабируемость. Созданный единожды образ системы для работы всей группы пользователей позволяет при минимальных затратах поддерживать легко масштабируемую сеть. Возможно быстрое создание любого количества новых рабочих мест.
- безопасность и отказоустойчивость. Компьютерный терминал, загружаясь, получает операционную систему «от производителя», настройка которой осуществляется только отделом информационной поддержки. Все модификации операционной системы и прикладных программ никак не влияют ни на других пользователей, ни на образ, хранящийся на сервере. Вся пользовательская информация хранится на сервере и регулярно резервируется, что увеличивает отказоустойчивость.
- защита от утечек информации – нет локальных носителей – нет возможности делать копии документов на съемные носители информации.
2. Входное имя пользователя (Login) — название учётной записи пользователя. Входному имени пользователя ставится в соответствиевнутренний идентификатор пользователя в системе (User ID,UID) — положительное целое число в диапазоне от 0 до65535, по которому в системе однозначно отслеживаются действия пользователя.
3. Учётные записи пользователей хранятся в файле/etc/passwd,который имеет следу-ющую структуру:login:password:UID:GID:GECOS:home:shell .
Например,учётные записи пользователейrootиivanв файле/etc/passwdмогутбыть записаны следующим образом:root:x:0:0:root:/root:/bin/bashivan:x:1000:100::/home/ivan:/bin/bash .
4. Начиная с версии 4.6, настройки рабочей среды хранятсяв реестреx fconf.
5. В многопользовательской модели пользователи делятся напользователей с обычными правамии администраторов. Входному имени пользователя ставится в соответствие внутренний идентификатор пользователя в системе (User ID,UID) — положительное целое число в диапазоне от 0 до 65535, по которому в системе однозначно отслеживаются действия пользователя.
6. Полномочия пользователей с административными правами обычно не ограничены. В многопользовательской модели пользователи делятся напользователей с обычными правамии администраторов. Пользователь с обычными правами может производить действия с элементами операционной системы только в рамках выделенного ему пространства и ресурсов, не влияя на жизнеспособность самой операционной системыи работу других пользователей. 
7. Процедура регистрации в системе обязательна для Linux. Каждый пользователь операционный системы имеет определенные ограничения на возможные с его стороны действия: чтение, изменение, запуск файлов,а так же на ресурсы: пространствона файловой системе, процессорное время для выполнение текущих задач (процессов).При этом действия одного пользователя не влияютна работу другого.Такая модель разграничения доступа к ресурсам операционной системы получила название многопользовательской.
8. Учётная запись пользователя содержит:
- входное имя пользователя (Login Name);
- пароль (Password);
- внутренний идентификатор пользователя (User ID);
- идентификатор группы (Group ID);
- анкетные данные пользователя (General Information);
- домашний каталог (Home Dir);
- указатель на программную оболочку (Shell).
9. Входному имени пользователя ставится в соответствиевнутренний идентификатор пользователя в системе (User ID,UID) — положительное целое число в диапазоне от 0 до65535, по которому в системе однозначно отслеживаются действия пользователя.
Пользователю можетбыть назначена определенная группа для доступа к некоторымресурсам, разграничения прав доступа к различным файлам и директориям. Каждаягруппа пользователей в операционной системе имеетсвой идентификатор—Group ID(GID).
10. Анкетные данные пользователя (General Information или GECOS) являются необязательным параметром учётной записи и могут содержать реальное имя пользователя (фамилию,имя),адрес,телефон.
11. Для каждого пользователя организуется домашний каталог, где хранятся его данныеи настройки рабочей среды.
В домашнем каталоге пользователя хранятся данные (файлы) пользователя,настройки рабочего стола и других приложений. Содержимое домашнего каталога обычно недоступно другим пользователям с обычными правами и не влияет на работу и настройки рабочей среды других пользователей. 
12. Мой домашний каталок: /afs/.dk.sci.pfu.edu.ru/home/t/b/tbkonovalova (узнаём с помощью команды pwd)
13. Администратор имеет возможность изменить содержимое домашнего каталогапользователя.
14. Учётные записи пользователей хранятся в файле/etc/passwd, который имеет следующую структуру: login:password:UID:GID:GECOS:home:shell
15. Для того, чтобы посмотреть содержимое файла /etc/shadow : изначально поле пароля содержало хеш пароля и использовалось для аутентификации.Однако из соображений безопасности все пароли были перенесены в специальный файл /etc/shadow, недоступный для чтения обычным пользователям. Поэтому в файле /etc/passwdполеpassword имеет значение x.
Символ* в поле password некоторой учётной записи в файле /etc/passwd означает, что пользователь не сможет войти в систему.
16. Виртуальные консоли — реализация концепции многотерминальной работы в рамках одного устройства. Мне кажется, что в данном контексте слово "виртуальный" означает реализованный программно, симулированный, имитированный с помощью компьютера.
17. Данная программа управляет доступом к физическим и виртуальным терминалам (tty).
18. Весь процесс взаимодействия пользователя с системой с момента ре-гистрации до выхода называетсясеансом работы.
19. Toolkit (Tk,«набор инструментов»,«инструментарий») — кроссплатформенная библиотека базовых элементов графического интерфейса, распространяемая с открытыми исходными текстами.
20. Используются следующие основныетулкиты: 
- GTK+ (сокращение от GIMP Toolkit) — кроссплатформенная библиотека элементов интерфейса;
- Qt—кросс - платформенный инструментарий разработки программного обеспеченияна языке программирования C++. GTK+ состоит из двух компонентов:
- GTK—содержит набор элементов пользовательского интерфейса (таких, как кнопка, список, поле для вводатекста ит.п.) для различных задач;
- GDK — отвечает за вывод информации на экран, может использовать для этого X Window System, Linux Framebuffer, WinAPI.

# Выводы

В ходе выполнения данной лабораторной работы я познакомился с операционной системой Linux, получил практические навыки работы с консолью и некоторыми графическими менеджерами рабочих столов операционной системы.
