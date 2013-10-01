Cloud Commander версія 0.4.0 [![NPM version][NPMIMGURL]][NPMURL] [![Dependency Status][DependencyStatusIMGURL]][DependencyStatusURL] [![Build Status][BuildStatusIMGURL]][BuildStatusURL]
===============
###[Головна][MainURL] [Блог][BlogURL] [Демо-версія][DemoURL]
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
[DemoURL]:                  http://io.cloudcmd.io "Демо-версія"
**Cloud Commander** - хмарковий файловий менеджер з консоллю та редактором.




![Cloud Commander](https://raw.github.com/coderaiser/cloudcmd/dev/img/logo/cloudcmd.png "Cloud Commander")

[![Flattr][FlattrIMGURL]][FlattrURL]

Переваги
---------------
- повна сумісність з браузерами *(іе6+,хром,сафарі,опера,фаєрфокс)*;
- чуйний дизайн
- одноразове завантаження сторінки, *and then just one-time json-dir-listings loading
(з можливістю оновлення).*
- кешування прочитаних папок *to localStorage (for now)
(тож якщо щось станеться з сигналом або ми втратимо зв'язок з мережею, ми
цілком зможемо працювати з кешованою копією папок)*;
- прив'язка клавіш
- disabled js support *(працює в режимі обмеження)*.


**Cloud Commander** використовує усі переваги Js, так що при вимкнутому Js,
він переходить в *обмежений режим*.


Особливості обмеженого режиму
---------------
- без прив'язки до клавіш
- без локального кешування
- повне завантаження усієї веб сторінки (зі стилями, js-скриптами, html-сторінками тощо).

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
- **Ctrl + d**          - очистити локальний кеш (в тому числі, вміст папки // wich contains dir contents)
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

Гарячі клавіші переглядача
---------------
- **F3**                - відкрити
- **Esc**               - закрити

Гарячі клавіші редактора
---------------
- **F4**                - відкрити
- **Ctrl + s**          - зберегти
- **Esc**               - закрити

Меню
---------------
Натискання на праву клавішу мишки, викликає меню з наступними пунктами:
- Перегляд
- Редагування
- Змінити назву
- Знищити
- Вивантажити до (Dropbox, Github, GDrive)
- Завантажити
- Новий (Файл, Папка, з хмарки)

Встановлення
---------------
[![NPM_INFO][NPM_INFO_IMG]][NPM_INFO_URL]

**Cloud Commander** встановлюється дуже просто.
Все що вам потрібно: 
- встановити [node.js](http://nodejs.org/ "node.js")
- [завантажити](https://github.com/coderaiser/cloudcmd/archive/master.zip)
і розпакувати або просто клонувати репозиторій з github (гітхабу):

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

Налаштування
---------------
Всі головні налаштування можна встановити в config.json.
```js
{
    "api_url"           :"/api/v1",
    "appcache"          : false,    /* cache files for offline use              */
    "analytics"         : true,     /* google analytics suport                  */
    "localStorage"      : true,     /* cache directory data                     */
    "minification" : {              /* minification of js,css,html and img      */
        "js"    : false,            /* minify module neaded                     */
        "css"   : false,            /* npm i minify                             */
        "html"  : true,
        "img"   : false
    },
    "cache"             : true,
    "logs"              : false,     /* logs or console ouput                    */
    "show_keys_panel"   : true,      /* show classic panel with buttons of keys  */
    "server"            : true,      /* server mode or testing mode              */
    "socket"            : true       /* enable web sockets                       */
    "port"              : 8000,      /* http port or null(default)               */
    "sslPort"           : 443,       /* https port or null(default)              */
    "ip"                : null,      /* ip or null(default)                      */
    "ssl"               : false      /* should use https?                        */
    "rest"              : true       /* enable rest interface                    */
}
```

Сервер
---------------
Standard practices say no non-root process gets to talk to
the Internet on a port less than 1024.В любому випадку, Я раджу Вам
запускати Cloud Commander не під рутом. Як це зробити?!
Існує декілька простих і швидких шляхів. Один з них - просування портів через iptables. // One of them is port forwarding by iptables.
Просто запустіть[shell/addtables.sh](shell/addtables.sh) для стандартних опцій.

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

If you would want to get things back just clear rules ( **1** and **2** it's rules numbers,
in your list they could differ).

```sh
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -D PREROUTING 1
@:/tmp/cloudcmd (dev) $ sudo iptables -t nat -D PREROUTING 2
```

To run Cloud Commander as daemon in linux you could set **log** to true in config and
do something like this:
    
    nohup node cloudcmd

Авторизація
---------------
Cloud Commander може авторизовувати клієнтів через openID на GitHub (ГітХаб).
Все що для цього потрібно - All things that should be done is must be added **id** and **secret** of application
from github settings page and added to **config.json** (id just) and env varible (secret)
with names: *github_id*, *github_secret*, *dropbox_key*, *dropbox_secret* etc.
For more information see **config.json** and **shell/seret.bat** *(on win32)*
or **shell/secret.sh** *(on nix)*.


Запуск
---------------
Для запуску **Cloud Commander** потрібна лише одна команда:
    
    node cloudcmd
або на Windows

    cloudcmd

Після цього, Cloud Commander читає інформацію порта з файлу налаштувань [config.json](json/config.json#L17) і запускає сервер
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
[jq-consoleURL]:            //github.com/replit/jq-console‎ "jq-console"
[githubURL]:                //github.com/michael/github "github"
[dropbox-jsURL]:            //github.com/dropbox/dropbox-js "dropbox-js"
[jqueryURL]:                //jquery.com

Contributing
---------------
If you would like to contribute - send pull request to dev branch.
Getting dev version of **Cloud Commander**:

    git clone git://github.com/coderaiser/cloudcmd.git
    git checkout dev

It is possible thet dev version Cloud Commander will needed dev version of Minify,
so to get it you should type a couple more commands:

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
MIT [license](LICENSE "ліцензія").

Щира подяка:
---------------
[Elena Zalitok](http://vk.com/politilena "Олені Заліток") за
[logo](img/logo/cloudcmd.png "логотип") та [favicon](img/favicon/favicon.png "фавіконку").
