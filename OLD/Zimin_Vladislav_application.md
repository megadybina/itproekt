﻿# Зимин Владислав - "karasique"
### Группа: 10 - МИ - 2
### Электронная почта: vlad_zimin2@mail.ru
### VK: https://vk.com/porolonoviy_gusar


**[ НАЗВАНИЕ ПРОЕКТА ]**

"karasique" 

**[ ПРОБЛЕМНОЕ ПОЛЕ ]**

Игровой процесс соревновательных онлайн-игр может показаться некоторым игрокам несколько надоедающим ввиду его однообразности и DOTA 2 не исключение. Данный проект направлен не только на устранение этой проблемы, но и на создание интерактивного способа получения информации о вселенной DOTA 2, погружения в её "лор"(от англ. Lore - история). 
Продукт будет предоставлять пользователям следующие возможности:
* Возможность узнать историю о героях и о мире DOTA, как от самих героев, так и из различных носителей информации, таких как книги, свитки, артефакты, приобретаемые за вирутальные монеты, либо получаемые в процессе выполнения заданий
* Удобный способ получения сведений об основных механиках игры в доступном виде
* Выполнение заданий или квестов, как в Discord, так и в самой DOTA 2
* Возможность выбора случайного героя, случайной роли в команде, случайной сборки снаряжения и т.д.
* Возможность испытать разные подходы к игровому процессу DOTA 2 и, возможно, открыть для себя что-то новое
 
И решать следующие проблемы:
* Неудобность большинства ныне существующих баз данных о DOTA 2
* Неправильная оценка новичками важности основных механик игры, что нередко приводит к поражениям в матчах и проблеме, описанной в пункте 3
* Потеря интереса к DOTA 2 у игроков

Окончательный продукт будет представлять собой бота для программы Discord, способного откликаться на определенные команды, заданные пользователем. Он будет размещен в открытый доступ, чтобы любой желающий мог добавить его на свой сервер. Таким образом все участники сервера, на котором находится бот, будут иметь возможность принять участие в ролевой игре, либо получить сведения о DOTA 2, без необходимости использовать браузер (это может оказаться особенно полезным для пользователей с малым количеством оперативной памяти т.к. некоторым браузерам свойственно использователь до 1Гб оперативной памяти!).

**[ ПОТЕНЦИАЛЬНАЯ АУДИТОРИЯ ]**

Продукт может показаться интересным любому любителю ролевых игр, даже не играющему в DOTA 2. Потенциальной аудиторией могут являться как новички, так и бывалые игроки DOTA. 

**[ АППАРАТНЫЕ ТРЕБОВАНИЯ ]** 

Discord – мультиплатформенная программа. Она может быть запущена на смартфонах и на компьютерах, а также облачную версию можно запустить через большинство бразуеров, тем не менее, на разработку это никак не влияет. Основные условия, необходимые для  пользования продуктом – возможность ввода команд с клавиатуры или любым другим способом и подключение к Интернету.

* IOS – версия 10.0 и выше, 100 Мб свободного места [Примечание: IPhone с экраном 3.5" и менее не поддерживаются.]
* Android – версия 4.1 Jellybean и выше, 100 Мб свободного места
* Облачная версия – Google Chrome, Firefox, Opera, Microsoft Edge 17
* Mac OS X – версия 10.10 Yosemite и выше, 1 Гб оперативной памяти и 100 Мб свободного дискового пространства
* Windows 7 – 1 Гб оперативной памяти и 100 Мб свободного дискового пространства 
* Linux – Ubuntu 16.04 [Примечание: поддерживается только 64-битная архитектура]

Чтобы воспользоваться полным функционалом продукта пользователю потребуется DOTA 2, однако, это не является обязательным условием пользования. Минимальные требования для DOTA 2:

 Windows 7 и выше:
 * 4 Гб оперативной памяти 
 * 15 Гб свободного дискового пространства
 * Графический процессор nVidia GeForce 8600/9600GT и выше / ATI/AMD Radeon HD2600/3600 и выше
 * Процессор Intel или AMD 2.8 ГГц и выше

Mac OS X Mavericks 10.9 и выше:
 * 4 Гб оперативной памяти 
 * 15 Гб свободного дискового пространства
 * Графический процессор nVidia 320M/ Radeon HD 2400/Intel HD 3000
 * Процессор Intel или AMD 2.8 ГГц и выше

Linux Ubuntu 12.04 и выше:
 * 4 Гб оперативной памяти 
 * 15 Гб свободного дискового пространства
 * Графический процессор: nVidia GeForce 8600/9600GT и выше / ATI/AMD Radeon HD2600/3600 и выше
 * Процессор Intel или AMD 2.8 ГГц и выше

**[ ФУНКЦИОНАЛЬНЫЕ ТРЕБОВАНИЯ ]**

* Создание наиболее полной базы данных о вселенной DOTA 2
* Интерактивный способ получения информации о вселенной DOTA 2
* Дополнение игрового процесса заданиями 
* Возможность предложить игроку новые способы игры в DOTA 2
* Возможность показать игроку все стороны и аспекты игрового процесса DOTA 2

**[ ПОХОЖИЕ ПРОДУКТЫ ]**

Анализ аналогичных проектов показал, что ни один из существующих ботов не объединяет в себе черты финальной версии разрабатываемого продукта. Не было найдено ни одного бота, который мог бы дать пользователю всю информацию об игровом процессе DOTA 2 и о её вселенной. Также не было выявлено ни одного бота сочетающего в себе RPG и одновременно способного давать пользователю задания, выполнение которых происходит прямо в DOTA 2.

**[ ИНСТРУМЕНТЫ РАЗРАБОТКИ ]**

*	Python 3.7
* Сторонние модули discord.py, requests, html2text и bs4 для python

**[ ЭТАПЫ РАЗРАБОТКИ ]**

* Создание денежной системы 
* Создание функции проверки выполнения заданий(квестов), выполняемых в DOTA 2
*	Создание и написание кода для квестов и других методов заработка виртуальной валюты, не требующих использования сторонних программ
* Создание базы знаний со сведениями о вселенной DOTA
*	Разработка удобного для пользования и интуитивно-понятного интерфейса
*	Написание документации с описанием всех команд и их описанием
*	Тестирование, отладка
*	Подготовка проекта к защите

**[ ВОЗМОЖНЫЕ РИСКИ ]**

* Сложность осуществления проверки выполнения заданий
*	Ограниченность базы квестов и,как следствие, потеря интереса пользователей к продукту
*	Трудности с созданием удобного пользовательского интерфейса 