---
layout: default
lang:
 - name: English
   link: http://cloudcmd.io
   translation: Англійською
 
 - name: Ukrainian
   link: http://ua.cloudcmd.io
   translation: Українською
 
 - name: Russian
   link: http://ru.cloudcmd.io
   translation: Російською

hideDownloadButtons: true
---

Cloud Commander 4.6.0
===============
###[Головна][MainURL] [Блог][BlogURL] Наживо(![JitSu][JitSu_LIVE_IMG] [JitSu][JitSuURL], ![Heroku][Heroku_LIVE_IMG] [Heroku][HerokuURL])
[NPM_INFO_IMG]:             https://camo.githubusercontent.com/254a020afe689842501ef5a79c04ba909f9b29d2/68747470733a2f2f6e6f6465692e636f2f6e706d2f636c6f7564636d642e706e673f646f776e6c6f6164733d7472756526267374617273 "npm install cloudcmd"
[MainURL]:                  http://cloudcmd.io "Головна"
[BlogURL]:                  http://blog.cloudcmd.io "Блог"
[JitSuURL]:                 http://cloudcmd.jit.su "JitSu"
[HerokuURL]:                http://cloudcmd.herokuapp.com/ "Heroku"
[JitSu_LIVE_IMG]:           https://status-io.cloudcmd.io/host/cloudcmd.jit.su/img/txt.png "JitSu"
[HEROKU_LIVE_IMG]:          https://status-io.cloudcmd.io/host/cloudcmd.herokuapp.com/img/txt.png "Heroku"

[DWORD]:                    https://github.com/cloudcmd/dword "Editor based on CodeMirror"
[EDWARD]:                   https://github.com/cloudcmd/edward "Editor based on Ace"
[EDWARD_KEYS]:              https://github.com/cloudcmd/edward/#hot-keys "Edward Hot keys"

**Cloud Commander** - двопанельний веб файл менеджер з консоллю та редактором. Допоможе вам керувати сервером та працювати з файлами, каталогами і програмами в браузері на будь-якому комп'ютері, смартфоні або планшеті.

![Cloud Commander](http://cloudcmd.io/img/logo/cloudcmd.png "Cloud Commander")

Переваги
---------------
- Відкритий код (**MIT License**).
- Має дві класичні панелі.
- Можливість **авторизації**.
- Клієнт працює у веб браузері.
- Сервер працює під **Windows**, **Linux** та **Mac OS**.
- Може використовуватись локально або віддалено.
- Підлаштовується під розмір екрану.
- **Два вбудовані редактори** з підтримкою **підсвітки синтаксису**: [Dword][DWORD] та [Edward][EDWARD].
- **Консоль** з підтримкою стандартного командного рядка ОС.
- Написаний на **JavaScript/Node.js**.
 
Встановлення
---------------

**Cloud Commander** встановлюється дуже просто:

- встановити [node.js](http://nodejs.org/ "node.js") або [io.js](https://iojs.org/ "io.js"), якщо ви цього ще не зробили.
- встановити ```cloudcmd``` через npm:
 
```sh
npm i cloudcmd -g
```

![NPM_INFO][NPM_INFO_IMG]

Запуск
---------------
Для запуску наберіть в консолі:

```sh
cloudcmd
```

**Cloud Commander** підтримує параметри командного рядка:

|Параметр                   |Дія
|:--------------------------|:--------------------------------------------
| `-h, --help`              | допомога
| `-v, --version`           | вивести версію і вийти
| `-s, --save`              | зберегти налаштування
| `-o, --online`            | вантажити скрипти з віддалених серверів
| `-a, --auth`              | увімкнути авторизацію
| `-u, --username`          | вказати ім'я користувача
| `-p, --password`          | вказати пароль
| `-c, --config`            | шлях до файлу налаштувань
| `--editor`                | вказати редактор: "dword" або "edward"
| `--root`                  | встановити кореневий каталог
| `--prefix`                | встановити url префікс
| `--port`                  | вказати порт
| `--minify`                | увімкнути мініфікацію
| `--progress`              | показувати статус файлових операцій
| `--no-server`             | не запускати сервер
| `--no-auth`               | вимкнути авторизацію
| `--no-online`             | вантажити скрипти з локального серверу
| `--no-minify`             | вимкнути мініфікацію
| `--no-progress`           | не показувати статус файлових операцій

Якщо не задано параметрів, Cloud Commander читає інформацію з `~/.cloudcmd.json` і використовує стандартний порт звідти (`8000` по замовчуванню), якщо змінних з іменами `PORT` або `VCAP_APP_PORT` не існує.

Для початку роботи, наберіть в адресному рядку вашого браузера:

```
http://localhost:8000
```

Оновлення
---------------
Якщо ви встановили Cloud Commander за допомогою `npm`, зупиніть додаток і переустановіть його:

```sh
npm update cloudcmd -g
```

Після цього знову запустіть додаток, почистіть кеш вашого браузеру та оновіть сторінку.

Гарячі клавіші
---------------

|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F1`                  | допомога
| `F2`                  | змінити назву
| `F3`                  | переглянути
| `Shift + F3`          | перегляд в `markdown`
| `F4`                  | редагувати
| `F5`                  | копіювати
| `F6`                  | змінити назву/перемістити
| `F7`                  | новий каталог
| `Shift + F7`          | новий файл
| `Shift + Delete`      | знищити без підтвердження
| `F8`, `Delete`        | знищити обраний файл
| `F9`                  | меню
| `F10`                 | налаштування
| `(*)`                 | виділити/зняти виділення з усього
| `(+)`                 | розширити виділення
| `(-)`                 | звузити виділення
| `Ctrl + x`            | вирізати в буфер
| `Ctrl + с`            | копіювати в буфер
| `Ctrl + v`            | вставити з буфера
| `Ctrl + r`            | оновити
| `Ctrl + d`            | очистити локальний кеш, що містить лістінг каталогів
| `Ctrl + a`            | виділити усі файли на панелі
| `Ctrl + u`            | поміняти панелі місцями
| `Up`, `Down`, `Enter` | пересування файловою системою
| `Alt + Left/Right`    | показати вміст каталогу під курсором у цільовій панелі
| `Alt + g`             | перейти до каталогу
| `Ctrl + \`            | перейти до кореневого каталогу
| `Tab`                 | переміщення між панелями
| `Page Up`             | вгору на одну сторінку
| `Page Down`           | вниз на одну сторінку 
| `Home`                | на початок списку 
| `End`                 | в кінець списку
| `Space`               | обрати поточний файл (і отримати розмір каталогу)
| `Insert`              | обрати поточний файл (і перейти до наступного)
| `Shift + F10`         | контекстне меню
| `~`                   | консоль
| `Ctrl + Click`        | відкрити файл в новій вкладці

Перегляд
---------------
![View](http://cloudcmd.io/img/screen/view.png "View")

### Можливості
- Переглянути зображення.
- Переглянути текстові файли.
- Програти аудіо.
- Програти відео.

### Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F3`                  | відкрити
| `Esc`                 | закрити

Редактор
---------------
![Edit](http://cloudcmd.io/img/screen/edit.png "Edit")

### Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F4`                  | відкрити
| `Esc`                 | закрити

[Гарячі клавіші Edward][EDWARD_KEYS].

Консоль
---------------
![Консоль](http://cloudcmd.io/img/screen/console.png "Консоль")

### Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `~`                   | відкрити
| `Ctrl + p`            | вставити шлях поточного каталогу
| `Esc`                 | закрити

[Гарячі клавіші console](https://github.com/cloudcmd/console#hot-keys).

Налаштування
---------------
![Налаштування](http://cloudcmd.io/img/screen/config.png "Налаштування")

###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F10`                 | відкрити
| `Esc`                 | закрити

Коли Ви змінюєте одну з опцій, файл `~/.cloudcmd.json` може бути збережений.
Їх можна змінювати особисто в любому текстовому редакторі.
Опис опцій:

```js
{
    "auth"              : false,     /* дозволити http авторизацію                                  */
    "username"          : "root",    /* ім'я користувача для авторизації                            */
    "password"          : "toor",    /* хеш пароль в sha-1 для авторизації                          */
    "algo"              : "sha512WithRSAEncryption", /* криптографічний алгоритм                    */
    "editor"            : "edward",  /* стандартний, може бути "dword" або "edward"                 */
    "diff"              : false,     /* при збереженні - відсилає патч, а не повний файл            */
    "zip"               : false,     /* zip текст пере посиланням / unzip перед збереженням         */
    "notifications"     : false,     /* показувати сповіщення, коли вкладка не активна              */
    "localStorage"      : true,      /* локальне сховище                                            */
    "buffer"            : true,      /* буфер для копіювання файлів                                 */
    "dirStorage"        : true,      /* зберігаті лістинг каталогів в localStorage                  */
    "minify"            : false,     /* мініфікація js, css, html та зображень                      */
    "cache"             : true,      /* додати контроль кешу                                        */
    "online"            : true,      /* загрузити файли js з cdn або Local path                     */
    "showKeysPanel"     : true,      /* показати класичну панель з кнопками функціональних клавіш   */
    "port"              : 8000,      /* http порт                                                   */
    "ip"                : null,      /* ip чи null(за замовчуванням)                                */
    "root"              : "/",       /* кореневий каталог                                           */
    "prefix"            : "",        /* url префікс                                                 */
    "progress"          : true       /* показувати статус файлових операцій                         */
}
```

Меню
---------------
![Menu](http://cloudcmd.io/img/screen/menu.png "Меню")
Натискання на праву клавішу мишки, викликає меню з наступними пунктами:

- Перегляд
- Редагування
- Змінити назву
- Видалити
- Запакувати
- Видобути
- Вивантажити в хмарку
- Завантажити
- Вирізати
- Копіювати
- Вставити
- Новий (Файл, Каталог)
- Вивантажити
- Вивантажити з хмарки
- Виділити все / зняти виділення
- Вийти (доступно якщо увімкнуто `авторизацію`)
 
###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F9`                  | відкрити
| `Esc`                 | закрити

Режим однієї панелі
---------------
Cloud Commander може працювати в режимі однієї панелі, у випадку, коли розмір екрану не дає змоги розмістити другу панель.
Таке може статися коли Ви працюєте з файловим менеджером із мобільного засобу, планшету або у маленькому вікні браузера.

![Режим однієї панелі](http://cloudcmd.io/img/screen/one-panel-mode.png "Режим однієї панелі")

Використання у ролі Middleware
---------------

Cloud Commander можна використовувати як middleware для `node.js` додатків, що побудовані на  [socket.io](http://socket.io "Socket.IO") та [express](http://expressjs.com "Express"):

```js
var http        = require('http'),
    cloudcmd    = require('cloudcmd'),
    express     = require('express'),
    io          = require('socket.io'),
    app         = express(),
    
    PORT        = 1337,
    
    server,
    socket;
    
server = http.createServer(app);
socket = io.listen(server);

app.use(cloudcmd({
    
    socket: socket,      /* використовується Config'ом, Edit'ом (не обов'язково) та Console'ллю (обов'язково)   */
    config: {                /* дані налаштуваннь (не обов'язково)                                              */
        prefix: '/cloudcmd', /* основний URL або функція що повертає основний URL (не обов'язково)              */
    }
}));

server.listen(PORT);
```

Сервер
---------------
Зазвичай процеси, що запущено з правами не root не можуть прослуховувати порти нижче ніж 1024.
В будь-якому випадку, краще запускати Cloud Commander не під рутом. Як це зробити?
Існує декілька простих і швидких шляхів. Один з них - просування портів через iptables.

###Iptables
Просто запустіть `shell/addtables.sh` для стандартних опцій.

```sh
iptables -t nat -L # look rules before
iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 8000
iptables -t nat -A PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 4430
iptables -t nat -L # look rules after
```

Ви маєте побачити щось на зразок ( **8000** та **4430** мають бути в config як **port** і **sslPort** )

```
target     prot opt source               destination
REDIRECT   tcp  --  anywhere             anywhere             tcp dpt:http redir ports 8000
REDIRECT   tcp  --  anywhere             anywhere             tcp dpt:https redir ports 4430
```

Якщо захочете все повернути, просто очистіть правила ( **1** та **2** це номера правил,
у вашому випадку вони можуть відрізнятися).

```sh
iptables -t nat -D PREROUTING 2
iptables -t nat -D PREROUTING 1
```

###nginx
Візьміть [nginx](http://nginx.org/ "nginx"). В Linux це можна зробити наступним чином:

```sh
sudo apt-get install nginx #for ubuntu and debian
```

І зробіть хост файл **/etc/nginx/sites-enabled/io.cloudcmd.io**
( *io.cloudcmd.io* ваше доменне ім'я) з вмістом:

```sh
server {
    listen 80;
    client_max_body_size 100m;
    server_name io.cloudcmd.io;
    access_log /var/log/nginx/io.cloudcmd.io.access.log;
    location / {
        proxy_pass    http://127.0.0.1:8000/;
    }
}
```

Якщо ви бажаєте додати **SSL**, додайте декілька рядків в розділ серверу:

```sh
server {
    listen 443;
    client_max_body_size 100m;
    ssl                  on;
    ssl_certificate      /home/coderaiser/cloudcmd/ssl/ssl.crt;
    ssl_certificate_key  /home/coderaiser/cloudcmd/ssl/ssl.key;
    server_name io.cloudcmd.io;
    access_log /var/log/nginx/io.cloudcmd.io.access.log;
    location / {
        proxy_pass    http://127.0.0.1:8000/;
    }
}
```

Якщо вам потрібне перенаправлення з **http** до **https**, просто зробіть так:

```sh
server {
    listen 80;
    server_name admin.cloudcmd.io;
    rewrite ^ https://io.cloudcmd.io$request_uri? permanent; #301 redirect
    access_log /var/log/nginx/io.cloudcmd.io.access.log;
}
```

```sh
# create symlink of this file
ln -s ./sites-enabled/io.cloudcmd.io ./sites-available
# restart nginx
/etc/init.d/nginx restart
```

Історія версій
---------------
- *2015.09.28*, **[v4.6.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.6.0.tar.gz)**
- *2015.09.27*, **[v4.5.7](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.7.tar.gz)**
- *2015.09.24*, **[v4.5.6](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.6.tar.gz)**
- *2015.09.23*, **[v4.5.5](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.5.tar.gz)**
- *2015.09.22*, **[v4.5.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.4.tar.gz)**
- *2015.09.16*, **[v4.5.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.3.tar.gz)**
- *2015.09.03*, **[v4.5.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.2.tar.gz)**
- *2015.08.28*, **[v4.5.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.1.tar.gz)**
- *2015.08.26*, **[v4.5.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.5.0.tar.gz)**
- *2015.08.25*, **[v4.4.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.4.0.tar.gz)**
- *2015.08.21*, **[v4.3.5](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.5.tar.gz)**
- *2015.08.19*, **[v4.3.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.4.tar.gz)**
- *2015.08.17*, **[v4.3.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.3.tar.gz)**
- *2015.08.17*, **[v4.3.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.2.tar.gz)**
- *2015.08.13*, **[v4.3.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.1.tar.gz)**
- *2015.08.11*, **[v4.3.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.3.0.tar.gz)**
- *2015.07.24*, **[v4.2.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.2.0.tar.gz)**
- *2015.07.23*, **[v4.1.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.1.2.tar.gz)**
- *2015.07.23*, **[v4.1.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.1.1.tar.gz)**
- *2015.07.21*, **[v4.1.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.1.0.tar.gz)**
- *2015.07.13*, **[v4.0.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v4.0.0.tar.gz)**
- *2015.07.09*, **[v3.8.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.8.1.tar.gz)**
- *2015.07.06*, **[v3.8.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.8.0.tar.gz)**
- *2015.07.04*, **[v3.7.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.7.2.tar.gz)**
- *2015.07.04*, **[v3.7.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.7.1.tar.gz)**
- *2015.07.03*, **[v3.7.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.7.0.tar.gz)**
- *2015.07.01*, **[v3.6.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.6.0.tar.gz)**
- *2015.06.27*, **[v3.5.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.5.0.tar.gz)**
- *2015.06.22*, **[v3.4.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.4.0.tar.gz)**
- *2015.06.20*, **[v3.3.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.3.0.tar.gz)**
- *2015.06.12*, **[v3.2.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.2.0.tar.gz)**
- *2015.06.11*, **[v3.1.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.1.4.tar.gz)**
- *2015.06.11*, **[v3.1.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.1.3.tar.gz)**
- *2015.06.10*, **[v3.1.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.1.2.tar.gz)**
- *2015.06.09*, **[v3.1.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.1.1.tar.gz)**
- *2015.06.09*, **[v3.1.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.1.0.tar.gz)**
- *2015.06.04*, **[v3.0.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.0.4.tar.gz)**
- *2015.06.02*, **[v3.0.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.0.3.tar.gz)**
- *2015.05.31*, **[v3.0.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.0.2.tar.gz)**
- *2015.05.29*, **[v3.0.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.0.1.tar.gz)**
- *2015.05.28*, **[v3.0.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v3.0.0.tar.gz)**
- *2015.05.22*, **[v2.9.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.9.3.tar.gz)**
- *2015.05.22*, **[v2.9.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.9.2.tar.gz)**
- *2015.05.19*, **[v2.9.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.9.1.tar.gz)**
- *2015.05.15*, **[v2.9.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.9.0.tar.gz)**
- *2015.05.14*, **[v2.8.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.8.0.tar.gz)**
- *2015.04.24*, **[v2.7.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.7.1.tar.gz)**
- *2015.04.24*, **[v2.7.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.7.0.tar.gz)**
- *2015.04.17*, **[v2.6.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.6.0.tar.gz)**
- *2015.04.14*, **[v2.5.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.5.1.tar.gz)**
- *2015.04.09*, **[v2.5.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.5.0.tar.gz)**
- *2015.04.03*, **[v2.4.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.4.2.tar.gz)**
- *2015.03.28*, **[v2.4.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.4.1.tar.gz)**
- *2015.03.28*, **[v2.4.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.4.0.tar.gz)**
- *2015.03.26*, **[v2.3.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.3.1.tar.gz)**
- *2015.03.26*, **[v2.3.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.3.0.tar.gz)**
- *2015.03.19*, **[v2.2.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.2.1.zip)**
- *2015.03.13*, **[v2.2.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.2.0.zip)**
- *2015.02.02*, **[v2.1.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.1.0.zip)**
- *2014.12.09*, **[v2.0.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v2.0.0.zip)**
- *2014.11.21*, **[v1.5.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.5.1.zip)**
- *2014.11.19*, **[v1.5.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.5.0.zip)**
- *2014.11.05*, **[v1.4.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.4.1.zip)**
- *2014.10.28*, **[v1.4.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.4.0.zip)**
- *2014.10.02*, **[v1.3.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.3.2.zip)**
- *2014.09.22*, **[v1.3.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.3.1.zip)**
- *2014.09.18*, **[v1.3.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.3.0.zip)**
- *2014.08.29*, **[v1.2.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.2.0.zip)**
- *2014.07.18*, **[v1.1.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.1.1.zip)**
- *2014.07.10*, **[v1.1.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.1.0.zip)**
- *2014.07.03*, **[v1.0.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v1.0.0.zip)**
- *2014.06.16*, **[v0.9.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.9.2.zip)**
- *2014.06.11*, **[v0.9.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.9.1.zip)**
- *2014.06.10*, **[v0.9.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.9.0.zip)**
- *2014.04.28*, **[v0.8.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.8.4.zip)**
- *2014.03.19*, **[v0.8.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.8.3.zip)**
- *2014.03.03*, **[v0.8.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.8.2.zip)**
- *2014.02.13*, **[v0.8.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.8.1.zip)**
- *2014.02.13*, **[v0.8.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.8.0.zip)**
- *2013.12.09*, **[v0.7.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.7.0.zip)**
- *2013.11.08*, **[v0.6.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.6.0.zip)**
- *2013.10.17*, **[v0.5.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.5.0.zip)**
- *2013.09.27*, **[v0.4.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.4.0.zip)**
- *2013.08.01*, **[v0.3.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.3.0.zip)**
- *2013.04.22*, **[v0.2.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.2.0.zip)**
- *2013.03.01*, **[v0.1.9](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.9.zip)**
- *2012.12.12*, **[v0.1.8](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.8.zip)**
- *2012.10.01*, **[v0.1.7](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.7.zip)**
- *2012.08.24*, **[v0.1.6](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.6.zip)**
- *2012.08.06*, **[v0.1.5](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.5.zip)**
- *2012.07.27*, **[v0.1.4](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.4.zip)**
- *2012.07.19*, **[v0.1.3](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.3.zip)**
- *2012.07.14*, **[v0.1.2](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.2.zip)**
- *2012.07.11*, **[v0.1.1](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.1.zip)**
- *2012.07.09*, **[v0.1.0](//github.com/cloudcmd/archive/raw/master/cloudcmd-v0.1.0.zip)**

Щира подяка:
---------------
- [Polietilena](http://polietilena.github.io/ "Polietilena") за **logo** та **favicon**.
- [TarZak](https://github.com/tarzak)
    - Російський та український переклади;
    - налаштування: шаблон та стилі
