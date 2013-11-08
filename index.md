---
layout: default
---

Cloud Commander 0.6.0 [![NPM version][NPMIMGURL]][NPMURL] [![Dependency Status][DependencyStatusIMGURL]][DependencyStatusURL] [![Build Status][BuildStatusIMGURL]][BuildStatusURL]
===============
###[Головна][MainURL] [Блог][BlogURL] Наживо(![IO][IO_LIVE_IMG] [IO][IOURL], ![JitSu][JitSu_LIVE_IMG] [JitSu][JitSuURL], ![Heroku][Heroku_LIVE_IMG] [Heroku][HerokuURL] ![RunKite][RunKite_LIVE_IMG] [RunKite][RunKiteURL])
[NPMIMGURL]:                https://badge.fury.io/js/cloudcmd.png
[BuildStatusIMGURL]:        https://secure.travis-ci.org/coderaiser/cloudcmd.png?branch=master
[DependencyStatusIMGURL]:   https://gemnasium.com/coderaiser/cloudcmd.png
[FlattrIMGURL]:             http://api.flattr.com/button/flattr-badge-large.png
[NPM_INFO_IMG]:             https://nodei.co/npm/cloudcmd.png?downloads=true&&stars
[NPMURL]:                   http://badge.fury.io/js/cloudcmd
[BuildStatusURL]:           http://travis-ci.org/coderaiser/cloudcmd  "Build Status"
[DependencyStatusURL]:      https://gemnasium.com/coderaiser/cloudcmd "Dependency Status"
[FlattrURL]:                https://flattr.com/submit/auto?user_id=coderaiser&url=github.com/coderaiser/cloudcmd&title=cloudcmd&language=&tags=github&category=software "flattr"
[NPM_INFO_URL]:             https://npmjs.org/package/cloudcmd "npm"
[MainURL]:                  http://cloudcmd.io "Головна"
[BlogURL]:                  http://blog.cloudcmd.io "Блог"
[DemoURL]:                  http://io.cloudcmd.io "Демо"
[IOURL]:                    http://io.cloudcmd.io "IO"
[JitSuURL]:                 http://cloudcmd.jit.su "JitSu"
[HerokuURL]:                http://cloudcmd.herokuapp.com/ "Heroku"
[RunKiteURL]:               http://cloudcmd.apps.runkite.com/ "RunKite"
[IO_LIVE_IMG]:              http://status-ok.cloudcmd.io/host/io.cloudcmd.io "IO"
[JitSu_LIVE_IMG]:           http://status-ok.cloudcmd.io/host/cloudcmd.jit.su "JitSu"
[HEROKU_LIVE_IMG]:          http://status-ok.cloudcmd.io/host/cloudcmd.herokuapp.com "Heroku"
[RunKite_LIVE_IMG]:         http://status-ok.cloudcmd.io/host/cloudcmd.apps.runkite.com/ "RunKite"

**Cloud Commander** - хмарний файловий менеджер з консоллю та редактором.

![Cloud Commander](http://cdn.cloudcmd.io/img/logo/cloudcmd.png "Cloud Commander")

[![Flattr][FlattrIMGURL]][FlattrURL]

Переваги
---------------
- Відкритий код.
- Має дві стандартні панелі.
- Працює під Windows, Linux та Mac OS.
- Може використовуватись локально або віддалено.
- Має гарну консоль та редактор.
- Написано на JavaScript/Node.js.
 
Встановлення
---------------
[![NPM_INFO][NPM_INFO_IMG]][NPM_INFO_URL]

**Cloud Commander** встановлюється дуже просто.
Все що вам потрібно: 

- встановити [node.js](http://nodejs.org/ "node.js")
- [завантажити](https://github.com/coderaiser/cloudcmd/archive/master.zip)
і розпакувати або просто клонувати репозиторій з github:

```
    git clone git://github.com/coderaiser/cloudcmd.git
    cd cloudcmd
    node cloudcmd
```
або встановити в npm:
```
    npm i cloudcmd -g
    cloudcmd
```

Гарячі клавіші
---------------
В усіх сучасних веб оглядачах (окрім Інтернет Експлорера, бо він особливий) гарячі клавіші працюють.
Короткий список:

- **F1**                - допомога
- **F2**                - змінити назву обраного файлу
- **F3**                - переглянути
- **F4**                - редагувати
- **F5**                - копіювати
- **F6**                - змінити назву/перемістити
- **F7**                - нова папка
- **F8, Delete**        - знищити обраний файл
- **F9**                - меню
- **Ctrl + r**          - оновити вміст папки
- **Ctrl + d**          - очистити локальний кеш, що містить вміст папки
- **Alt  + q**          - вимкнути прив'язку клавіш
- **Alt  + s**          - відновити усі прив'язки клавіші
- **Ctrl + a**          - виділити (обрати) усі файли на панелі
- **up, down, enter**   - пересування файловою систему (навігація по файловій системі)
- **Tab**               - змінити поточну панель // move thru panels
- **Page Up**           - вгору на одну сторінку // up on one page
- **Page Down**         - вниз на одну сторінку // down on one page
- **Home**              - на початок списку // to begin of list
- **End**               - в кінець списку // to end of list
- **Shift + Delete**    - знищити без запиту (підтвердження) // remove without prompt
- **Insert**            - обрати поточнний файл
- **Shift + F10**       - контекстне меню
- **~**                 - консоль

Редактор
---------------
[Демо](http://io.cloudcmd.io/fs/etc#/edit/passwd "Edit")
![Edit](/img/screen/edit.png "Edit")


###Гарячі клавіші
- **F4**                - відкрити
- **Ctrl + s**          - зберегти
- **Esc**               - закрити
 
Детальніше [Ace keyboard shortcuts](https://github.com/ajaxorg/ace/wiki/Default-Keyboard-Shortcuts "Ace keyboard shortcuts").

Console
---------------
[Demo](http://io.cloudcmd.io#/console "Console")
![Console](/img/screen/console.png "Console")

###Гарячі клавіші
- **~**                 - відкрити
- **Esc**               - закрити

Налаштування
---------------
[Demo](http://io.cloudcmd.io#/config "Config")
![Console](/img/screen/config.png "Config")

###Гарячі клавіші
- **F10**               - відкрити
- **Esc**               - закрити

Меню
---------------
[Demo](http://io.cloudcmd.io#/menu "Menu")
![Menu](/img/screen/menu.png "Menu")
Натискання на праву клавішу мишки, викликає меню з наступними пунктами:

- Перегляд
- Редагування
- Змінити назву
- Знищити
- Zip файл
- Обрати все
- Вивантажити до (Dropbox, Github, GDrive)
- Завантажити
- Новий (Файл, Папка, з хмарки)
 
###Гарячі клавіші
- **F9**                - відкрити
- **Esc**               - закрити

Налаштування
---------------
Всі головні налаштування можна встановити в config.json.

```js
{
    "api_url"           :"/api/v1",
    "appcache"          : false,     /* кешувати файли для оффлайнового використання               */
    "analytics"         : true,      /* підтримка google analytics                                 */
    "localStorage"      : true,      /* кешування вмісту папки                                     */
    "minify"            : true,      /* minification js,css,html та img                            */
    "cache"             : true,      /* додати контроль кешу                                       */
    "online"            : true,      /* загрузити файли js з cdn або Local path                    */
    "logs"              : false,     /* виводити в логи чи в консоль                               */
    "show_keys_panel"   : true,      /* показати класичну панель з кнопками функціональних клавіш  */
    "server"            : true,      /* режим сервера чи тестування                                */
    "socket"            : true       /* увімкнути web сокети                                       */
    "port"              : 8000,      /* http порт чи null(за замовчанням)                          */
    "sslPort"           : 443,       /* https порт чи null(за замовчанням)                         */
    "ip"                : null,      /* ip чи null(за замовчуванням)                               */
    "ssl"               : false      /* використовувати https?                                     */
    "rest"              : true       /* увімкнути решту інтерфейса                                 */
}
```

Якщо ви змінили **config** і хочете продовжувати оновлюватись via git,
вам потрібно виконати наступну команду в корневій директорії **Cloud Commander**:

```
git update-index --assume-unchanged json/config.json
```

Щоб повернутися до відстежування:

```
git update-index --no-assume-unchanged json/config.json
```

Сервер
---------------
Зазвичай процеси, що запущено правами не root не можуть звертатися до портів нижче ніж 1024.
В любому випадку, Я раджу Вам запускати Cloud Commander не під рутом. Як це зробити?!
Існує декілька простих і швидких шляхів. Один з них - просування портів через iptables. // One of them is port forwarding by iptables.
Просто запустіть [shell/addtables.sh](http://github.com/coderaiser/cloudcmd/blob/master/shell/addtables.sh) для стандартних опцій.

```sh
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -L # look rules before
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 8000
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -A PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 4430
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -L # look reles after
```
Ви маєте побачити щось таке ( **8000** and **4430** should be in config as **port** and **sslPort** )

    target     prot opt source               destination
    REDIRECT   tcp  --  anywhere             anywhere             tcp dpt:http redir ports 8000
    REDIRECT   tcp  --  anywhere             anywhere             tcp dpt:https redir ports 4430

Якщо захочете все повернути, просто очистіть правила ( **1** та **2** це номера правил,
у вашому випадку вони можуть відрізнятися).

```sh
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -D PREROUTING 1
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -D PREROUTING 2
```

Для запуску Cloud Commander під daemon в linux встановіть **log** в "істину" в config-файлі і
зробіть щось на зразок:
    
    nohup node cloudcmd

Авторизація
---------------
Cloud Commander може авторизовувати клієнтів через openID на GitHub.
Все що для цього потрібно - додати **id** і **secret** додатків зі сторінки 
налаштувань github в **config.json** (id just) and env varible (secret)
з іменами: *github_id*, *github_secret*, *dropbox_key*, *dropbox_secret* і т.д.
Для додаткової інформації, дивіться **config.json** та **shell/seret.bat** *(для win32)*
або **shell/secret.sh** *(для nix)*.


Запуск
---------------
Для запуску **Cloud Commander** потрібна лише одна команда:
    
    node cloudcmd
або на Windows

    cloudcmd

Після цього, Cloud Commander читає інформацію порта з файлу налаштувань [config.json](http://github.com/coderaiser/cloudcmd/blob/master/json/config.json#L17) і запускає сервер
на цьому порті ( **8000**, за замовчуванням ),якщо змінних портів не існує( *cloud9*, *cloudfoundry* and *nodester* ).
Тоді просто наберіть в броузері

    http://127.0.0.1:8000
або

    http://localhost:8000
Оновлення
---------------
**Cloud Commander** дуже часто оновлюється.
Оновлення відбувається автоматично, але його можна виконати власноруч
за допомогою декількох команд в папці Cloud Commander:

    git pull
перевірити наявність нової версії на npm

    npm info cloudcmd

і якщо нова версія існує

    npm r cloudcmd
    npm i cloudcmd

Додаткові модулі
---------------
**Серверна частина Cloud Commander** не використовує додаткові модулі для основного функціоналу.
Але для мінімізації та оптимізації додатково можна 
призначити (та встановити) модулі [Minify] (https://github.com/coderaiser/minify "Minify")
та [socket.io] (https://github.com/LearnBoost/socket.io "Socket.IO").

Щоб встановити додаткові модулі, напишіть знаходячись в папці **Cloud Commander**:

    npm i

Розширення
---------------
**Cloud Commander** створено з можливістю легкого розширення основного функціоналу.
Щоб розширити функціонал Cloud Commander, використовуйте такі модулі:

- [Ace]                     [AceURL]
- [FancyBox]                [FancyBoxURL]
- [jQuery-contextMenu]      [jQuery-contextMenuURL]
- [jq-console]              [jq-consoleURL]
- [github]                  [githubURL]
- [dropbox-js]              [dropbox-jsURL]
- [jquery]                  [jqueryURL]

[AceURL]:                   //ace.ajax.org/ "Ace"
[FancyBoxURL]:              //github.com/fancyapps/fancyBox "FancyBox"
[jQuery-contextMenuURL]:    //github.com/medialize/jQuery-contextMenu "jQuery-contextMenu"
[jq-consoleURL]:            //github.com/replit/jq-console "jq-console"
[githubURL]:                //github.com/michael/github "github"
[dropbox-jsURL]:            //github.com/dropbox/dropbox-js "dropbox-js"
[jqueryURL]:                //jquery.com

Долучитися до проекту
---------------
Якщо ви хочете долучитися до проекту - відправте pull запит в dev гілку.
Отримання dev версії **Cloud Commander**:

    git clone git://github.com/coderaiser/cloudcmd.git
    git checkout dev

Можливо вам знадобиться dev версія Minify,
щоб отримати її, вам потрібно ввести декілька команд:

    cd node_modules
    rm -rf minify
    git clone git://github.com/coderaiser/minify
    git checkout dev

Історія версій
---------------
- *2013.09.27*, **[v0.4.0](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.4.0.zip)**
- *2013.07.01*, **[v0.3.0](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.3.0.zip)**
- *2013.04.22*, **[v0.2.0](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.2.0.zip)**
- *2013.03.01*, **[v0.1.9](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.9.zip)**
- *2012.12.12*, **[v0.1.8](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.8.zip)**
- *2012.10.01*, **[v0.1.7](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.7.zip)**
- *2012.08.24*, **[v0.1.6](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.6.zip)**
- *2012.08.06*, **[v0.1.5](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.5.zip)**
- *2012.07.27*, **[v0.1.4](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.4.zip)**
- *2012.07.19*, **[v0.1.3](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.3.zip)**
- *2012.07.14*, **[v0.1.2](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.2.zip)**
- *2012.07.11*, **[v0.1.1](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.1.zip)**
- *2012.00.00*, **[v0.1.0](//github.com/coderaiser/cloudcmd-archive/raw/master/cloudcmd-v0.1.0.zip)**

Ліцензія
---------------
MIT [license](http://github.com/coderaiser/cloudcmd/blob/master/LICENSE "ліцензія").

Щира подяка:
---------------
[Polietilena](http://polietilena.github.io "Polietilena") за
[logo](http://github.com/coderaiser/cloudcmd/blob/master/img/logo/cloudcmd.png "логотип") та [favicon](http://github.com/coderaiser/cloudcmd/blob/master/img/favicon/favicon.png "фавіконку").
