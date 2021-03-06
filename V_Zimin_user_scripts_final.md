# Владислав Зимин - "yasha"
# Пользовательские сценарии

### Группа: 11 - МИ - 2
### Электронная почта: vlad_zimin2@mail.ru 
### VK: https://vk.com/porolonoviy_gusar 


### [ Сценарий 1 - Добавление бота на сервер ]
* Пользователь входит в / создает учетную запись Discord на сайте https://discordapp.com
* Пользователь открывает веб-версию Discord или устанавливает программу Discord соответствующей версии на свою ОС
* Пользователь создает сервер в Discord
* Если сервер уже существует то пользователь должен убедиться, что он имеет права администратора на этом сервере. В  противном случае пользователь должен запросить у администратора сервера вышеназванные права, либо попросить администратора добавить бота на сервер собственноручно
* Пользователь переходит по **ссылке приглашения бота на сервер** (находится в конце файла; ближе к завершению работы над проектом будет размещена на сайте https://discordbots.org и/или аналогах)
* Пользователь выбирает в выпадающем списке сервер, на который он хочет добавить бота
* Если сервера нет в списке, то назад к шагу 4
* Пользователь подтверждает действие вводом капчи
* Бот автоматически заходит на сервер и пользователь получает уведомление об этом в текстовый канал сервера, к которому присоединился бот
* Пользователю будет предложено выбрать язык бота (русский/английский), по умолчанию - английский
* Пользователю будет предложено выбрать префикс для команд, например: "!", "-","$" и т.д.(по умолчанию - "!") [Это необходимо для того, чтобы  не происходило одновременное выполнение команд разных ботов, имеющих одинаковые префиксы команд]
* Бот уведомит пользователя о том, что он может получить список команд, написав команду `!help` в любой текстовый канал сервера(подсказка о команде `!help` будет также находится под именем бота в списке участников сервера)

[Примечание: чтобы использовать бота необязательно писать команды в текстовый канал сервера - можно отправлять команды в личные сообщения бота, но для этого все равно необходимо, чтобы бот находился в списке участников сервера пользователя, чтобы была возможность отправить ему сообщение, нажав ПКМ по боту в списке и выбрав пункт "Сообщение". В этом документе будут рассматриваться сценарии, когда пользователь пишет команды в текстовый канал сервера и когда установлен префикс команд "!". Стоит иметь в виду, что результат работы команд не будет отличаться в зависимости от того куда было отправлено сообщение, но если все же будут добавлены команды, работающие только при отправлении в текстовый канал сервера, что маловероятно, то об этом будет указано около соответствующей команды в разделе `!help`]

### [ Сценарий 2 - Получение информации о боте и командах ]
* Пользователь вводит команду `!help` в любой текстовый чат сервера, на котором присутствует бот
* На первой странице выведенного сообщения находится информация о самой команде `!help`, то есть, различные пояснения, например: "При введении команды `!help <название команды>` будет выведено описание соответствующей команды", а также уведомление о том, что "реагировать" на сообщения нужно только после смены реакции под сообщением пользователя с некоторой командой с ⏳ на ✔
* Под сообщением добавляется ботом несколько реакций для быстрого доступа к соответствующему разделу, например, реакция с изображением книжки выведет описание команд, связанных с базой данных о DOTA 2 (подобные реакции будут в каждом разделе, некоторые из них тематические, например, реакция с изображением книжки - иконка предмета из DOTA 2; основные описаны ниже)
* При нажатии на реакцию 🤖 выводится краткое описание самого бота и его функционала
* При нажатии на реакцию ↩ выводится начальная страница, то есть, описание команды `!help` и реакции для перехода в разделы
* При нажатии на реакцию 🔙 выводится предыдущая страница, если такая существует
* Для некоторых команд установлена проверка реагирующего, например:
    * Вносить изменения в настройки бота (смена языка/префикса, установленного на сервере) с помощью команды `!settings` могут только пользователи с правами администратора на сервере
    * Выбирать действия при просмотре информации о игроке или матче могут только пользователи, создавшие запрос на вывод соответствующей информации (бот поддерживает одновременное создание нескольких запросов даже в одном текстовом канале)
* Также пользователь может добавить название некоторых команд после `!help` (Пример: `!help hero`). При использовании такой команды выводится подробное описание команды и выходных данных.
* Для получения префикса сервера необходимо `@mention` бота (написать @ и имя бота) в любой текстовый чат сервера.
* В статусе бота в списке участников сервера всегда находятся подсказки о получении префикса сервера и списка команд.

### [ Сценарий 3 - Использование функций рандома ]
* Пользователь вводит команду в любой текстовый чат сервера, на котором присутствует бот. Содержание сообщения зависит от введенной команды
* При введении команды `!random tip` пользователю будет дан случайный совет из списка подсказок, связанных как с игровым процессом, так и с настройками игры(Пример:"Be careful when crossing the river into enemy territory.|Будьте осторожны при пересечении реки на территорию противника." Язык зависит от выбора пользователя[сценарий 1])
* При введении пользователем команды `!random hero` ему будет предложено сыграть на случайном герое DOTA 2
* К сообщению будет приложена фотография героя, чтобы новичкам было легче найти его. Пример:
![Пример](https://github.com/megadybina/itproekt/blob/master/resources/randomhero.png)
* При введении пользователем команды `!random mode` ему будет предложен случайный игровой режим (Пример: "Abillity draft")
* При введении пользователем команды `!random build` ему будет предложена случайная сборка на героя указанного в сообщении непосредственно после команды (Пример сообщения: "!randombuild Abaddon")
* Если в сообщении не указано имя героя или в нем допущены ошибки - пользователю будет сообщено об этом
* При введении пользователем команды `!random role` ему будет предложена случайная роль в команде (Пример: "Поддержка")
* При введении пользователем команды `!flip` ботом будет "подброшена" тематическая монетка и выведена выпавшая сторона
  
### [ Сценарий 4 - Получение информации о DOTA 2 ]
* Пользователь вводит команду `!info` или `!tome` в любой текстовый канал сервера, на котором присутствует бот
* В текстовый канал сервера выводится содержание интерактивной энциклопедии, в котором указаны ее разделы
* Под сообщением ботом создаются "реакции", при нажатии на которые, сообщение редактируется в соответствии с запросом(Пример: при нажатии пользователем на :arrow_right: откроется следующая страница энциклопедии)
* Пользователь может получить информацию о последнем патче, о механиках игры(Пример: механика атрибута "Броня"), ролях в команде и т.д.,
используя эту энциклопедию.
* Пользователь может получить информацию о конкретном герое, его способностях и атрибутах, введя команду `!hero <Имя героя>`
* Пользователь может получить информацию о предмете DOTA 2, введя команду `!item <Название предмета>`
* Пользователь может получить информацию о способности DOTA 2, введя команду `!ability <Название способности>`

### [ Сценарий 5 - Получение информации об обновлении DOTA 2 ]
* При введении пользователем команды `!help patch`, выводится описание команды, то есть её синтаксис и возможные выходные данные
* При использовании `!patch` выводится список доступных патчей, которые можно использовать в `<номер патча>`
* При использовании `!patch <имя героя/предмета> <номер патча>` выводятся изменения `<имя героя/предмета>` в патче `<номер патча>`
* При использовании `!patch <имя героя/предмета>` выводятся изменения `<имя героя/предмета>` в последнем досутпном патче 
* При использовании `!patch <номер патча>` выводится список досутпных изменений в патче `<номер патча>`
* Если доступны общие изменения, то об этом указано в заголовке сообщения, возвращяемого при использовании `!patch <номер патча>`. Чтобы их просмотреть нужно использовать `!patch general <номер патча>`
**Новые изменения патча становятся досутпны в течение нескольких дней после выхода обновления**

### [ Сценарий 6 - Получение информации о матче ]
* Пользователь вводит команду `!matchinfo <ID матча>` в любой текстовый чат сервера, на котором присутствует бот
* Если не введен ID матча или ID введен неверно, то бот уведомляет об этом пользователя и просит ввести команду заново с корректным ID
* В текстовый канал сервера выводится информация о матче, о строениях и всех героях.
* Ботом создаются "реакции" с изображением героев, которых выбрали участники матча, при нажатии на которое будет выводится более конкретная информация о соответствующем игроке, например, какие предметы купил, сколько совершил убийств и т.д.
* Ботом создается "реакция" с изображением карты, при нажатии на которую будет создана и отправлена пользователю миникарта с расположением построек в конце матча и распределением героев по линиям в начале. Темная расцветка постройки - обозначение того, что она была разрушена.
* Также создается реакция ❌, при нажатии на которую удаляются все реакции
* При введении пользователем команды `!lastmatchinfo` в текстовый канал сервера будет выведена информация о последнем матче, в котором участвовал пользователь
* Если в базе данных отсутствует ID профиля DOTA 2 пользователя, то бот отправит сообщение с просьбой пользователя ввести свой ID
* Информация о последнем матче пользователя будет выведена при повторном введении команды `!lastmatchinfo`

### [ Сценарий 7 - Поиск способностей по критериям ]
* Пользователь вводит команду `!abs <критерий 1> .. <критерий n>` в любой текстовый чат сервера, на котором присутствует бот
* Вместо `<критерий n>` пользователь вводит критерий(-ии) к необходимым ему способностям в виде `<название критерия><оператор><значение>`. Примеры: `!abs damage>550`, `!abs stun_dur>=5 сooldown<=20` и т.д.
* Бот выводит список героев и названия их способностей, подходящих под заданные критерии
* Если не найдено ни одной способности, удовлетворяющей заданным критериям, бот сообщает об этом пользователю
* Если поиск по какому-либо из критериев невозможен, то этот критерий игнорируется
* Пользователь может просмотреть список доступных критериев с помощью `!help abs`
________________________________________________________________________________________________________________________________________
[ссылка приглашения бота на сервер]
https://discordapp.com/oauth2/authorize?client_id=537272694018932754&permissions=1074261056&scope=bot
