# Fika - A multiplayer mod for SPT

<details open>
	<summary>Содержимое</summary>
	<ol>
		<li><a href="#что-такое-fika">Что такое Fika</a></li>
		<li><a href="#лицензия">Лицензия</a></li>
		<li>
           	<a href="#требования">Требования</a>
            <ul>
                <li><a href="#хост">Хост</a></li>
                <li><a href="#клиент">Клиент</a></li>
            </ul>
        </li>
        <li><a href="#системные-требования">Системные требования</a></li>
		<li>
	            <a href="#установка">Установка</a>
	            <ul>
	                <li><a href="#хост-с-использованием-перенаправления-портов">Хост с использованием перенаправления портов</a></li>
	                <li><a href="#хост-с-использованием-впн">Хост с использованием ВПН</a></li>
	                <li><a href="#клиент-с-использованием-перенаправления-портов">Клиент с использованием перенаправления портов</a></li>
	                <li><a href="#клиент-с-использованием-впн">Клиент с использованием ВПН</a></li>
		    </ul>
		</li>
        </li>
        <li><a href="#особенности-и-настройка">Особенности и настройки</a></li>
	        <ul>		
                    <li><a href="#особенности-и-что-делать">Особенности и что делать</a></li>
                    <li><a href="#настройки-клиента">Настройки клиента</a></li>
                    <li><a href="#настройки-сервера">Настройки сервера</a></li>
	        <ul>			    
              </li>
        </ol>
</details>

## Что такое Fika

**Fika** это мод для **SPT** позволяющий играть вам вместе с вашими друзьями. Он использует P2P-UDP соединение для современного и производительного опыта. Основные цели Fika это: производительность, точность и поддержка модов. Fika сейчас поддерживается командой Fika team.
Вы можете присоединится [здесь](https://discord.gg/project-fika)!

## Лицензия

<img src="https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc-sa.png" alt="cc by-nc-sa" width="196" height="62" style="float:right">

Этот проект распространяется под лицензией [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode.en).

- Вы можете только распространять Fika и его производные до тех пор пока правильно указываете авторство и не используете для коммерческого использования.
- Вы не можете монетизировать ваш сервер в виде донатов или платных услуг.
- Вы не можете хостить большие публичные сервера, Fika сделан для кооперативной игры с вашими друзьями.
- Вы не можете копировать и/или воспроизводить **художественный материал** Fika который сделан нашими художниками или артистами без их соглашения.

## Требования

Fika требует общие знания о компьютерах, компьютерных сетях и SPT. Если эти пункты вам не знакомы, этот проект не для вас. Пожалуйста попробуйте понять и уважать это.

### Хост

- Роутер и Интернет-провайдер поддерживающие **Перенаправление портов** или **UPnP**
- TCP Порт 6969 для SPT Сервера
- UDP Порт 25565 для P2P траффика (если используете UPnP это не требуется)
- Функциональный SPT, совпадающий с версией Fika которую вы используете
- Доступ к вашему Widows Firewall (Брандмауэр)
- Интернет соединение, рекомендуется со скоростью как минимум 20 Мбит/с на прием и передачу. Каждый клиент в среднем потребляет 400 килобит/с.

### Клиент

- Роутер и Интернет-провайдер поддерживающие **Перенаправление портов** или **UPnP** | **ПРИМЕЧАНИЕ**: Это необходимо только если вы собираетесь хостить внутри игры
- UDP Порт Открытый для P2P траффика, стандартный 25565 (если используете UPnP это не требуется) | **ПРИМЕЧАНИЕ**: Тоже что и пункт выше
- Функциональный SPT, совпадающий с версией Fika которую вы используете
- Доступ к вашему Windows Firewall (Брандмауэр)
- Интернет соединение, рекомендуется со скоростью как минимум 20 Мбит/с на прием и передачу.

### Обоим

- Последняя версия Fika

## Системные требования

Это рекомендации для наилучшей игры:

- **Процессор**: i7 8700k / Ryzen 7 2700x
- **Видеокарта**: GTX 1060 / RX 580
- **ОЗУ** 16 Гб минимум, 32 GB крайне рекомендуется
- **Диск**: SSD обязателен, не рассчитывайте на поддержку запуская Fika на HDD

Лучше всего для Fika (и SPT в общем) будет иметь мощные Процессор и ОЗУ.

## Установка

### Хост с использованием перенаправления портов

Прежде чем начать, убедитесь, что вы сделали перенаправление портов какие указаны в Требованиях. Мы не будем помогать вам с перенаправлением портов у вас. Если вы не имеете доступа в вашему роутеру или не можете сделать перенаправление портов, используйте ВПН.

**Настройки Брандмауэра**

1. Порт 6969 **TCP** перенаправленный на вашем роутере (входящий и исходящий траффик)
2. Порт 25565 **UDP** перенаправленный на вашем роутере (входящий и исходящий траффик)
3. При запросе от Windows, разрешить ***все*** соединения в вашем Брандмауэре
4. Если возникли проблемы, мы рекомендуем вам разрешить EscapeFromTarkov.exe (для всех) и Server.exe (хост сервера) для входящих и исходящих подключений в вашем расширенном брандмауэре Windows (Windows Advanced Firewall).

**Общая установка**

1. [Скачайте последнюю версию плагина Fika](https://github.com/project-fika/Fika-Plugin/releases/latest) и [последнюю версию Fika server mod](https://github.com/project-fika/Fika-Server/releases/latest)
2. Перейдите в вашу папку с установленным SPT и распакуйте в нее архив
3. Запустите `Server.exe` дождитесь пока он сгенерирует файлы конфигурации для Fika, затем закройте его
4. Вернитесь в основную папку SPT, перейдите в `SPT_Data\Server\configs` и откройте текстовым редактором `http.json`
5. Измените значение для `ip` на `0.0.0.0`, затем сохраните файл и закройте его
6. Перейдите в папку `user\mods\fika-server\assets\configs` и откройте `fika.jsonc`
7. Измените любые из этих параметров по своему вкусу.
    - **useBtr**: должен ли БТР появляться или нет когда вы играете на Улицах Таркова
    - **friendlyFire**: должен ли быть включен огонь по своим
    - **dynamicVExfils**: автоматическое масштабирование мест в транспортных средствах в зависимости от количества игроков в рейде
    - **allowFreeCam**: позволяет игрокам переключать свободную камеру в рейде
    - **giftedItemsLoseFIR**: должны ли передаваемые между схронами вещи терять пометку Найдено в рейде
8. Запустите `Server.exe` и ждите окончания загрузки
    - Это то что вы должны увидеть при успешном запуске с примером WAN IP `70.60.150.90`:
    ```
    Started webserver at http://70.60.150.90:6969
    Started websocket at ws://70.60.150.90:6969
    Server is running, do not close while playing SPT, Happy playing!!
    ```
9. Запустите `Launcher.exe`
10. Ваши друзья могут присоединяться к вам используя ваш внешний IP, который можно определить с помощью сайта [IPv4.ICanHazIP](https://ipv4.icanhazip.com/) или [MyIP](https://myip.ru)

### Хост с использованием ВПН
Ваи понадобятся ВПН по типу `Hamachi`, `ZeroTier` или `Radmin`.

1. [Скачайте последнюю версию плагина Fika](https://github.com/project-fika/Fika-Plugin/releases/latest) и [последнюю версию Fika server mod](https://github.com/project-fika/Fika-Server/releases/latest)
2. Перейдите в вашу папку с установленным SPT и распакуйте в нее архив
3. Запустите `Server.exe` дождитесь пока он сгенерирует файлы конфигурации для Fika, затем закройте его
4. Вернитесь в основную папку SPT, перейдите в `SPT_Data\Server\configs` и откройте текстовым редактором `http.json`
5. Измените начение для `ip` на ваш IP из ВПН, затем сохраните файл и закройте его

Пример с ненастоящим адресом (**20.20.56.73**):
```json
{
	"ip": "20.20.56.73",
	"port": 6969,
	"webSocketPingDelayMs": 90000,
	"logRequests": true,
	"serverImagePathOverride": {	}
} 
```
6. Перейдите в папку `user\mods\fika-server\assets\configs` и откройте `fika.jsonc`
7. Измените любые из этих параметров по своему вкусу.
    - **useBtr**: должен ли БТР появляться или нет когда вы играете на Улицах Таркова
	- **friendlyFire**: должен ли быть включен огонь по своим
	- **dynamicVExfils**: автоматическое масштабирование мест в транспортных средствах в зависимости от количества игроков в рейде
	- **allowFreeCam**: позволяет игрокам переключать свободную камеру в рейде
    - **giftedItemsLoseFIR**: должны ли передаваемые между схронами вещи терять пометку Найдено в рейде
8. Запустите `Server.exe` и ждите окончания загрузки
    - Это то что вы должны увидеть при успешном запуске с IP использованным в шаге 5:
    ```
    Started webserver at http://20.20.56.73:6969
    Started websocket at ws://20.20.56.73:6969
    Server is running, do not close while playing SPT, Happy playing!!
    ```
9. Запустите `Launcher.exe` и нажмите 'Settings'/'Настройки'
10. Поле `URL` измените так чтобы оно соответствовало вашему IP ВПН. Используя пример из шага 5 оно должно выглядеть примерно так: `http://20.20.56.73:6969` (не забудьте удалить все лишние косые черты`/`)

### Клиент с использованием перенаправления портов

1. [Скачайте последнюю версию плагина Fika](https://github.com/project-fika/Fika-Plugin/releases/latest)
2. Перейдите в вашу папку с установленным SPT и распакуйте в нее архив
3. Запустите `Launcher.exe` и нажмите 'Settings'/'Настройки'
4. Поле `URL` измените чтобы адрес соответствовал внешнему IP Хоста (не забудьте удалить все лишние косые черты `/`)
5. Если хостите внутри игры, разрешите все соединения (публичные и приватные) по запросу от Брандмауэра Windows

### Клиент с использованием ВПН

1. [Скачайте последнюю версию плагина Fika](https://github.com/project-fika/Fika-Plugin/releases/latest)
2. Перейдите в вашу папку с установленным SPT и распакуйте в нее архив
3. Запустите `Launcher.exe` и нажмите 'Settings'/'Настройки'
4. Поле `URL` измените чтобы адрес соответствовал ВПН IP Хоста. Используя пример из шага 5 оно должно выглядеть примерно так: `http://20.20.56.73:6969` (не забудьте удалить все лишние косые черты`/`)
5. Если хостите внутри игры, разрешите все соединения (публичные и приватные) по запросу от Брандмауэра Windows

## Особенности и настройка

### Особенности и что делать
**Fika** позволяет вам создавать P2P сессии с вашими друзьями для кооперативной игры. Хост это тот с чьей стороны происходит наибольший контроль за внутриигровой логикой в процессе игры, такие как работа ИИ, минные поля, зоны снайперов, БТР, и так далее. Каждый клиент отвечает за свой урон, как по себе так и по ботам. Это означает что попадания по ботам будут отзывчивыми и быстрыми.

Чтобы создать рейд выберите карту и время, и затем нажмите на кнопку `Host Raid`. Выберите количество игроков для рейда (включая себя) и ждите пока завершится загрузка. После ее завершения другие игроки могут присоединится к вашей сессии, и когда все завершат загрузку игра автоматически начнется.

**Другие особенности Fika**
- Передача вещей
    - Нажмите ПКМ по предмету чтобы отправить его на другой аккаунт
    - Можно изменить через [Настройки Сервера](#sнастройки-сервера)
- Свободная камера (по умолчанию на клавишу `F9`)
    - В свободной камере вы можете переместится к местоположению камеры нажав `T`
    - Вы можете переместится к другим игрокам нажимая `Влево/Вправо` 
    - Вы можете прикрепить камеру к их голове с помощью кнопки `ПРОБЕЛ` когда перемещаетесь
    - Вы можете включить вид от их 3-го лица нажав `CTRL` когда перемещаетесь
    - Вы можете нажать клавишу `HOME` для временного отображения кнопок управления камерой
- Множитель урона по вам для критичных частей тела
- Динамически ИИ для хоста, который выключает ботов если никого нет рядом
- Настраиваемое количество ботов на карте
- Система куллинга для повышения производительности
- Настраиваемые уведомления (союзник погиб, босс убит игроком, и тд.)
- Система пингов позволяющая вам помечать зоны в игре для ваших союзников
- Полоска хп игрока для ваших союзников

Большая часть этих настроек доступна в [Настройки Клиента](#настройки-клиента).

### Настройки Клиента

Чтобы открыть ваши настройки клиента нажмите `F12` в игре. Перейдите в раздел `Fika Core` для изменения настроек

**Кооп**

- **Show Notifications**: Включает настраиваемые уведомления когда игрок умирает, покидает рейд, убивает босса, и тд.
- **Auto Extract**: Игрок автоматически покидает рейд вместо переключения на свободную камеру.
- **Show Extract Message**: Определяет когда показывать сообщения о выходе после смерти/выхода.

**Кооп | Настраиваемое**

- **Show Player Name Plates**: Показывать полоски ХП и имена.
- **Show HP% instead of bar**: Показывать ХП в процентах вместо полоски.
- **Show Player Faction Icon**: Показывать значок фракции игрока рядом с полоской ХП.
- **Name Plate Scale**: Изменяет размер плашек с именами.
- **Ping System**: Включает систему Пингов. Если включено вы можете получать и отправлять пинги нажимая соответствующую клавишу.
- **Ping Button**: Кнопка используемая для отправки пингов.
- **Ping Color**: Цвет вашего пинга который отображается у других игроков.
- **Ping Size**: Множитель размера пинга.
- **Play Ping Animation**: Автоматически проигрывать анимацию указывания при пинге. Может мешать геймплею.

**Кооп | Отладка**

- **Free Camera Button**: Кнопка используемая для включения свободной камеры.

**Производительность**

- **Dynamic AI**: Использование динамической системы ИИ, выключая ИИ когда они слишком далеко от игрока.
- **Dynamic AI Range**: Дальность с которой динамический ИИ будет выключаться.
- **Dynamic AI Rate**: Как часто динамическйи ИИ должен делать проверки расстояния до игроков.
- **Culling System**: Когда должна работать система куллинга. Когда игроки вне дистанции куллинга, их анимации будут упрощены. Это может крайне увеличить производительность в некоторых случаях.
- **Culling Range**: Дистанция с которой работает система куллинга для игроков.

**Производительность | Максимальное количество ботов**

- **Enforced Spawn Limits**: Принудительный лимит спавна ботов, убедитесь что это не превышает стандартные лимиты. Это, в основном, влияет при использовании модов или чего-то еще что влияет на лимит ботов.
- **Max Bots** `MAP`: Максимальное количетсво ботов которые могут быть активны одновременно на карте `MAP`. Полезно если у вас слабый компьютер. Поставьте 0 для отключения.

**Сеть**

- **Native Sockets**: NativeSockets для игрового траффика. Это использует прямые вызовы сокетов для отправки/получения для серьезного увеличения скорости и снижения GC pressure. Только для Windows/Linux и не всегда может работать.
- **Force IP**: Заставляет сервер при хостинге использовать этот IP-адрес при трансляции на серверную часть вместо автоматической попытки его получить. Оставьте поле пустым для отключения. Эта опция требуется при использовании ВПН, используйте ваш IP из ВПН.
- **Force Bind IP**: Заставляет сервер при хостинге использовать этот локальный IP-адрес при запуске сервера. Полезно если вы хостите игры через ВПН. Оставьте поле пустым для отключения. Эта опция требуется при использовании ВПН, используйте ваш IP из ВПН.
- **Auto Server Refresh Rate**: Каждые X секунд клиент будет опрашивать сервер на наличие игр в окне лобби.
- **UDP Port**: Порт используемый для игровых UDP пакетов.
- **Use UPnP**: Пытается открыть порты используя UPnP. Полезно если вы не можете открыть порты сами, но роутер поддерживает UPnP.
- **Connection Timeout**: Как долго ждать связи до тех пор пока она не будет расчитана потеряной.
- **Use NAT Punching**: Использовать проброс NAT при хосте рейда. Работает только с маршрутизаторами типа Fullcone NAT и требует, чтобы NatPunchServer был запущен на сервере SPT. UPnP, Force IP и Force Bind IP отключены в этом режиме.

**Геймплей**

- **Head Damage Multiplier**: X множитель урона получаемого в хитбокс головы. 0.2 = 20%
- **Armpit Damage Multiplier**: X множитель урона получаемого в хитбокс подмышек. 0.2 = 20%
- **Stomach Damage Multiplier**: Xмножитель урона получаемого в хитбокс живота. 0.2 = 20%
- **Disable Bot Metabolism**: Отключить метаболизм у ИИ, что бы избежать их смерти от усталости/дегидратации в течении долгих рейдов.
### Настройки Сервера

Настройки сервера могут быть найдены в папке `user\mods\fika-server\assets\configs`. Откройте `fika.jsonc` текстовым редактором.

```json
{
    "client": {
        "useBtr": true, // должен ли БТР появляться на улицах. По умолчанию: true
        "friendlyFire": true, // включен ли огонь по союзникам. По умолчанию: true
        "dynamicVExfils": false, // автоматическое масштабирование мест в транспортных средствах в зависимости от количества игроков в рейде отличное от стандартных 4. По умолчанию: false
        "allowFreeCam": false, // можно ли включать свободную камеру когда угодно. По умолчанию: false
        "allowItemSending": true // можно ли передавать вещи между схронами. По умолчанию: true
        "blacklistedItems": [], // ИД предметов которые нельзя передавать, к примеру: ["5c94bbff86f7747ee735c08f", "5c1d0f4986f7744bb01837fa"] Не разрешит отправлять ключи доступа и черные ключ-карты
        "forceSaveOnDeath": false, // if saving is forced upon death, preventing ALT+F4 cheese. По умолчанию: false
        "mods": {
            "required": [], // Требуемые сервером моды, если включего - должно всегда содержать стандартные библиотеки СПТ: ["com.SPT.custom", "com.SPT.singleplayer", "com.SPT.core", "com.SPT.debugging", "com.fika.core", "com.bepis.bepinex.configurationmanager"]
            "optional": [] // Не требуемые но допустимые моды
        },
        "useInertia": true, // Должна ли быть включена инерция. По умолчанию: true
        "sharedQuestProgression": false // Должна ли быть включена возможность общего прогресса по квестам. По умолчанию: false
    },
    "server": {
        "giftedItemsLoseFIR": true, // должны ли передаваемые вещи терять отметку найдено в рейде. По умолчанию: true
        "launcherListAllProfiles": false, // Должен ли лаунчер показывать все профили. По умолчанию: false
        "sessionTimeout": 5, // Как долго ждать серверу ответа на пинга клиента до обьявки того что соединение потеряно. По умолчанию: 5
        "showDevProfile": false, // Можно ли создать профиль разработчика. По умолчанию: false
        "showNonStandardProfile": false // Могут ли быть созданы не стандартные типы профилей. По умолчанию: false
    },
    "natPunchServer": {
        "enable": false, // Включать ли проброс NAT. По умолчанию: false
        "port": 6790, //Порт проброса NAT. По умолчанию: 6970
        "natIntroduceAmount": 1
    }
}
```
