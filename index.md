---
layout: default
lang:
 - name: English
   link: //cloudcmd.io
   translation: Англійською
 
 - name: Ukrainian
   link: //ua.cloudcmd.io
   translation: Українською
 
 - name: Russian
   link: //ru.cloudcmd.io
   translation: Російською

scripts:
 - https://ajax.googleapis.com/ajax/libs/jquery/3.0.0/jquery.min.js
 - https://cdnjs.cloudflare.com/ajax/libs/fancybox/2.1.5/jquery.fancybox.min.js
 - https://files.cloudcmd.io/js/view.js

styles:
 - https://cdnjs.cloudflare.com/ajax/libs/fancybox/2.1.5/jquery.fancybox.min.css

hideDownloadButtons: true
---

# Cloud Commander 19.1.10

### [Головна][MainURL] [Блог][BlogURL] [Підтримати](SupportURL)

[MainURL]:                  http://cloudcmd.io "Головна"
[BlogURL]:                  http://blog.cloudcmd.io "Блог"
[SupportURL]:               https://patreon.com/coderaiser "Patreon"

[DWORD]:                    https://github.com/cloudcmd/dword "Редактор базується на CodeMirror"
[EDWARD]:                   https://github.com/cloudcmd/edward "Редактор базується на Ace"
[DEEPWORD]:                 https://github.com/cloudcmd/deepword "Редактор базується на Monaco"
[EDWARD_KEYS]:              https://github.com/cloudcmd/edward/#hot-keys "Гарячі клавіші Edward" 
[TERMUX]:                   https://termux.com "Termux"

**Cloud Commander** - двопанельний веб файл менеджер з консоллю та редактором. Допоможе вам керувати сервером та працювати з файлами, каталогами і програмами в браузері на будь-якому комп'ютері, смартфоні або планшеті.

![Cloud Commander](//cloudcmd.io/img/logo/cloudcmd.png "Cloud Commander")

Переваги
---------------
- Відкритий код (**MIT License**).
- Має дві класичні панелі.
- Можливість **авторизації**.
- Клієнт працює у веб браузері.
- Сервер працює під **Windows**, **Linux**, **Mac OS** та **Android** (за допомогою [Termux][TERMUX]).
- Може використовуватись локально або віддалено.
- Підлаштовується під розмір екрану.
- **Три вбудовані редактори** з підтримкою **підсвітки синтаксису**: [Dword][DWORD], [Edward][EDWARD] та [Deepword][DEEPWORD].
- [Консоль](https://github.com/cloudcmd/console "Консоль") з підтримкою стандартного командного рядка ОС.
- Написаний на **JavaScript/Node.js**.
 
Встановлення
---------------

**Cloud Commander** встановлюється дуже просто:

- встановити останню версію [node.js](http://nodejs.org/ "node.js"), якщо ви цього ще не зробили.
- встановити `cloudcmd` через `npm`:
 
```sh
npm i cloudcmd -g
```

У разі халепи:

```sh
npm i cloudcmd -g --force
```

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
| `--html-dialogs`          | показувати html діалоги
| `--open`                  | відкрити веб браузер після старту сервера
| `--no-server`             | не запускати сервер
| `--no-auth`               | вимкнути авторизацію
| `--no-online`             | вантажити скрипти з локального серверу
| `--no-open`               | не відкривати веб браузер після старту сервера
| `--no-minify`             | вимкнути мініфікацію
| `--no-progress`           | не показувати статус файлових операцій
| `--no-html-dialogs`       | не використовувати html діалоги

Якщо не задано параметрів, Cloud Commander читає інформацію з `~/.cloudcmd.json` і використовує стандартний порт звідти (`8000` за замовчуванням), якщо змінних з іменами `PORT` або `VCAP_APP_PORT` не існує.

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
![Перегляд](//cloudcmd.io/img/screen/view.png "Перегляд")

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
![Редактор](//cloudcmd.io/img/screen/edit.png "Редактор")

### Гарячі клавіші

|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F4`                  | відкрити
| `Esc`                 | закрити

[Гарячі клавіші Edward][EDWARD_KEYS].

Консоль
---------------
![Консоль](//cloudcmd.io/img/screen/console.png "Консоль")

### Гарячі клавіші

|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `~`                   | відкрити
| `Ctrl + p`            | вставити шлях поточного каталогу
| `Esc`                 | закрити

[Гарячі клавіші console](https://github.com/cloudcmd/console#hot-keys).

Налаштування
---------------
![Налаштування](//cloudcmd.io/img/screen/config.png "Налаштування")

### Гарячі клавіші

|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F10`                 | відкрити
| `Esc`                 | закрити

Результат налаштування файлового менеджера записується в текстовий файл доступний для читання і редагування. Він називається `~/.cloudcmd.json` і містить наступні поля:

```js
{
    "auth"              : false,     /* дозволити http авторизацію                                  */
    "username"          : "root",    /* ім'я користувача для авторизації                            */
    "password"          : "toor",    /* хеш пароль в sha-1 для авторизації                          */
    "algo"              : "sha512WithRSAEncryption", /* криптографічний алгоритм                    */
    "editor"            : "edward",  /* стандартний, може бути "dword" або "edward"                 */
    "diff"              : false,     /* при збереженні - відсилає патч, а не повний файл            */
    "zip"               : false,     /* zip текст пере посиланням / unzip перед збереженням         */
    "localStorage"      : true,      /* локальне сховище                                            */
    "buffer"            : true,      /* буфер для копіювання файлів                                 */
    "dirStorage"        : true,      /* зберігаті лістинг каталогів в localStorage                  */
    "minify"            : false,     /* мініфікація js, css, html та зображень                      */
    "online"            : true,      /* загрузити файли js з cdn або Local path                     */
    "open"              : false,     /* відкрити веб браузер після старту сервера                   */
    "cache"             : true,      /* додати контроль кешу                                        */
    "showKeysPanel"     : true,      /* показати класичну панель з кнопками функціональних клавіш   */
    "port"              : 8000,      /* http порт                                                   */
    "ip"                : null,      /* ip чи null(за замовчуванням)                                */
    "root"              : "/",       /* кореневий каталог                                           */
    "prefix"            : "",        /* url префікс                                                 */
    "progress"          : true,      /* показувати статус файлових операцій                         */
    "htmlDialogs"       : true       /* показувати html діалоги                                     */
}
```

Меню
---------------
![Меню](//cloudcmd.io/img/screen/menu.png "Меню")

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
 
### Гарячі клавіші

|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F9`                  | відкрити
| `Esc`                 | закрити

Режим однієї панелі
---------------
Cloud Commander може працювати в режимі однієї панелі, у випадку, коли розмір екрану не дає змоги розмістити другу панель.
Таке може статися коли Ви працюєте з файловим менеджером із мобільного засобу, планшету або у маленькому вікні браузера.

![Режим однієї панелі](//cloudcmd.io/img/screen/one-file-panel.png "Режим однієї панелі")

Використання у ролі Middleware
---------------

Cloud Commander можна використовувати як middleware для `node.js` додатків, що побудовані на  [socket.io](http://socket.io "Socket.IO") та [express](http://expressjs.com "Express").

Створіть `package.json`:

```
npm init -y
```

Встановіть залежності:

```
npm i cloudcmd express socket.io -S
```

Та створіть `index.js`:

```js
const http = require('http');
const cloudcmd = require('cloudcmd');
const io = require('socket.io');
const app = require('express')();

const port = 1337;
const prefix = '/cloudcmd';

const server = http.createServer(app);
const socket = io.listen(server, {
    path: `${prefix}/socket.io`
});

const config = {
    prefix, // основний URL або функція що повертає основний URL (не обов'язково)
};

const plugins = [
    __dirname + '/plugin.js'
];

const filePicker = {
    data: {
        FilePicker: {
            key: 'key'
        }
    }
};

// перевизначити налаштування з json/modules.json
const modules = {
    filePicker,
};

app.use(cloudcmd({
    socket,  // використовується Config'ом, Edit'ом (не обов'язково) та Console'ллю (обов'язково)
    config,  // дані налаштуваннь (не обов'язково)
    plugins, // не обов'язково
    modules, // не обов'язково
}));

server.listen(port);
```

Сервер
---------------
Зазвичай процеси, що запущено з правами не root не можуть прослуховувати порти нижче ніж 1024.
В будь-якому випадку, краще запускати Cloud Commander не під рутом. Як це зробити?
Існує декілька простих і швидких шляхів. Один з них - просування портів через iptables.

### Iptables
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

### nginx
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

Розгортання
---------------
`Cloud Commander` з легкістю можна розгорнути на [Heroku](https://heroku.com/deploy?template=https://github.com/coderaiser/cloudcmd "Розгорнути на Heroku").

[![Розгорнути на Heroku](https://www.herokucdn.com/deploy/button.png "Розгорнути на Heroku")](https://heroku.com/deploy?template=https://github.com/coderaiser/cloudcmd)

Docker
---------------
`Cloud Commander` може бути використаний як [docker контейнер](https://hub.docker.com/r/coderaiser/cloudcmd/ "Docker контейнер"):

```sh
docker run -v ~:/root -v /:/mnt/fs -t -p 8000:8000 coderaiser/cloudcmd
```

Налаштування будуть читатися з домашнього каталогу, корінь файлової системи буде монтований у `/mnt/fs`,
`8000` порт буде виставлено у відповідності до мережевого порту головної системи.

Також Ви можете скористатися [docker compose](https://docs.docker.com/compose/ "Docker Compose") з `docker-compose.yml`:

```yml
version: '2'
services:
  web:
    ports:
      - 8000:8000
    volumes:
      - ~:/root
      - /:/mnt/fs
    image: coderaiser/cloudcmd
```

Коли створите файл, запустіть:

```sh
    docker-compose up
```

Долучайтесь
---------------
 
Існує багато способів долучитися до розробки `Cloud Commander`:
 
 - якщо ви знайшли баг або маєте ідею [створюйте issue](https://github.com/coderaiser/cloudcmd/issues/new "Створити issue");
 - якщо ви виправили баг, помилку в тесті або реалізували новий функціонал [створюйте pull request](https://github.com/coderaiser/cloudcmd/compare "Створити pull request");
 - якщо Ви володієте мовами Ви можете допомогти з [перекладом сайту](https://github.com/coderaiser/cloudcmd/wiki "Вікі спільноти Cloud Commander");

Історія версій
---------------
- *2026.01.20*, **[v19.1.10](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.10)**
- *2026.01.17*, **[v19.1.9](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.9)**
- *2026.01.17*, **[v19.1.8](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.8)**
- *2026.01.16*, **[v19.1.7](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.7)**
- *2026.01.16*, **[v19.1.6](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.6)**
- *2026.01.16*, **[v19.1.5](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.5)**
- *2026.01.15*, **[v19.1.4](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.4)**
- *2026.01.15*, **[v19.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.3)**
- *2026.01.14*, **[v19.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.2)**
- *2026.01.12*, **[v19.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.1)**
- *2025.12.31*, **[v19.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v19.1.0)**
- *2025.12.24*, **[v19.0.17](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.17)**
- *2025.12.05*, **[v19.0.16](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.16)**
- *2025.11.28*, **[v19.0.15](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.15)**
- *2025.11.27*, **[v19.0.14](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.14)**
- *2025.09.26*, **[v19.0.13](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.13)**
- *2025.09.25*, **[v19.0.12](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.12)**
- *2025.09.24*, **[v19.0.11](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.11)**
- *2025.09.23*, **[v19.0.10](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.10)**
- *2025.09.22*, **[v19.0.9](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.9)**
- *2025.09.20*, **[v19.0.8](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.8)**
- *2025.09.18*, **[v19.0.7](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.7)**
- *2025.09.17*, **[v19.0.6](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.6)**
- *2025.09.16*, **[v19.0.5](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.5)**
- *2025.09.15*, **[v19.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.4)**
- *2025.09.15*, **[v19.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.3)**
- *2025.09.14*, **[v19.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.2)**
- *2025.09.14*, **[v19.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.1)**
- *2025.09.14*, **[v19.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v19.0.0)**
- *2025.09.14*, **[v18.10.11](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.11)**
- *2025.09.14*, **[v18.10.10](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.10)**
- *2025.09.14*, **[v18.10.9](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.9)**
- *2025.09.13*, **[v18.10.8](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.8)**
- *2025.09.12*, **[v18.10.7](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.7)**
- *2025.09.12*, **[v18.10.6](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.6)**
- *2025.09.10*, **[v18.10.5](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.5)**
- *2025.09.09*, **[v18.10.4](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.4)**
- *2025.09.04*, **[v18.10.3](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.3)**
- *2025.09.04*, **[v18.10.2](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.2)**
- *2025.09.04*, **[v18.10.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.1)**
- *2025.09.02*, **[v18.10.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.10.0)**
- *2025.08.30*, **[v18.9.4](//github.com/coderaiser/cloudcmd/releases/tag/v18.9.4)**
- *2025.07.26*, **[v18.9.3](//github.com/coderaiser/cloudcmd/releases/tag/v18.9.3)**
- *2025.07.24*, **[v18.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v18.9.2)**
- *2025.07.06*, **[v18.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.9.1)**
- *2025.07.05*, **[v18.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.9.0)**
- *2025.07.04*, **[v18.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.8.1)**
- *2025.07.02*, **[v18.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.8.0)**
- *2025.04.10*, **[v18.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.7.1)**
- *2025.03.29*, **[v18.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.7.0)**
- *2025.02.03*, **[v18.6.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.6.1)**
- *2025.01.20*, **[v18.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.6.0)**
- *2025.01.20*, **[v18.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.5.0)**
- *2024.12.13*, **[v18.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.4.1)**
- *2024.11.22*, **[v18.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.4.0)**
- *2024.11.14*, **[v18.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.3.0)**
- *2024.11.06*, **[v18.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.2.1)**
- *2024.10.27*, **[v18.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.2.0)**
- *2024.08.17*, **[v18.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.1.0)**
- *2024.08.16*, **[v18.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v18.0.2)**
- *2024.08.16*, **[v18.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v18.0.1)**
- *2024.08.16*, **[v18.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v18.0.0)**
- *2024.08.16*, **[v17.4.4](//github.com/coderaiser/cloudcmd/releases/tag/v17.4.4)**
- *2024.07.27*, **[v17.4.3](//github.com/coderaiser/cloudcmd/releases/tag/v17.4.3)**
- *2024.07.03*, **[v17.4.2](//github.com/coderaiser/cloudcmd/releases/tag/v17.4.2)**
- *2024.05.06*, **[v17.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v17.4.1)**
- *2024.04.17*, **[v17.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v17.4.0)**
- *2024.04.03*, **[v17.3.3](//github.com/coderaiser/cloudcmd/releases/tag/v17.3.3)**
- *2024.03.29*, **[v17.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v17.3.2)**
- *2024.03.29*, **[v17.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v17.3.1)**
- *2024.03.29*, **[v17.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v17.3.0)**
- *2024.03.29*, **[v17.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v17.2.1)**
- *2024.03.22*, **[v17.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v17.2.0)**
- *2024.03.21*, **[v17.1.6](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.6)**
- *2024.03.20*, **[v17.1.5](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.5)**
- *2024.03.20*, **[v17.1.4](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.4)**
- *2024.03.18*, **[v17.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.3)**
- *2024.03.18*, **[v17.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.2)**
- *2024.03.16*, **[v17.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.1)**
- *2024.03.16*, **[v17.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v17.1.0)**
- *2024.03.12*, **[v17.0.7](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.7)**
- *2024.03.11*, **[v17.0.6](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.6)**
- *2024.03.11*, **[v17.0.5](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.5)**
- *2024.02.02*, **[v17.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.4)**
- *2024.02.01*, **[v17.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.3)**
- *2024.02.01*, **[v17.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.2)**
- *2024.01.25*, **[v17.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.1)**
- *2023.12.12*, **[v17.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v17.0.0)**
- *2023.12.08*, **[v16.18.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.18.0)**
- *2023.12.04*, **[v16.17.9](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.9)**
- *2023.12.04*, **[v16.17.8](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.8)**
- *2023.10.12*, **[v16.17.7](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.7)**
- *2023.09.22*, **[v16.17.6](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.6)**
- *2023.09.06*, **[v16.17.5](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.5)**
- *2023.09.05*, **[v16.17.4](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.4)**
- *2023.09.05*, **[v16.17.3](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.3)**
- *2023.09.04*, **[v16.17.2](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.2)**
- *2023.09.04*, **[v16.17.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.1)**
- *2023.09.04*, **[v16.17.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.17.0)**
- *2023.08.10*, **[v16.16.3](//github.com/coderaiser/cloudcmd/releases/tag/v16.16.3)**
- *2023.08.09*, **[v16.16.2](//github.com/coderaiser/cloudcmd/releases/tag/v16.16.2)**
- *2023.08.07*, **[v16.16.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.16.1)**
- *2023.07.09*, **[v16.16.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.16.0)**
- *2023.05.17*, **[v16.15.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.15.0)**
- *2023.03.21*, **[v16.14.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.14.1)**
- *2023.03.08*, **[v16.14.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.14.0)**
- *2023.01.30*, **[v16.13.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.13.1)**
- *2023.01.29*, **[v16.13.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.13.0)**
- *2023.01.29*, **[v16.12.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.12.0)**
- *2023.01.22*, **[v16.11.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.11.0)**
- *2023.01.19*, **[v16.10.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.10.0)**
- *2023.01.18*, **[v16.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.9.1)**
- *2023.01.17*, **[v16.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.9.0)**
- *2023.01.16*, **[v16.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.8.0)**
- *2023.01.15*, **[v16.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.7.0)**
- *2022.10.20*, **[v16.6.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.6.1)**
- *2022.10.09*, **[v16.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.6.0)**
- *2022.08.06*, **[v16.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.5.0)**
- *2022.07.20*, **[v16.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.4.1)**
- *2022.07.11*, **[v16.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.4.0)**
- *2022.07.02*, **[v16.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.3.1)**
- *2022.07.01*, **[v16.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.3.0)**
- *2022.06.17*, **[v16.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.2.0)**
- *2022.05.12*, **[v16.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.1.1)**
- *2022.04.23*, **[v16.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.1.0)**
- *2022.04.22*, **[v16.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v16.0.1)**
- *2022.02.19*, **[v16.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v16.0.0)**
- *2022.01.20*, **[v15.9.15](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.15)**
- *2022.01.13*, **[v15.9.14](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.14)**
- *2021.12.23*, **[v15.9.13](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.13)**
- *2021.12.16*, **[v15.9.12](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.12)**
- *2021.12.09*, **[v15.9.11](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.11)**
- *2021.12.04*, **[v15.9.10](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.10)**
- *2021.11.22*, **[v15.9.9](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.9)**
- *2021.08.09*, **[v15.9.8](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.8)**
- *2021.06.27*, **[v15.9.7](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.7)**
- *2021.06.13*, **[v15.9.6](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.6)**
- *2021.06.08*, **[v15.9.5](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.5)**
- *2021.04.05*, **[v15.9.4](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.4)**
- *2021.03.17*, **[v15.9.3](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.3)**
- *2021.03.16*, **[v15.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.2)**
- *2021.03.01*, **[v15.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.1)**
- *2021.03.01*, **[v15.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.9.0)**
- *2021.02.27*, **[v15.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.8.1)**
- *2021.02.23*, **[v15.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.8.0)**
- *2021.02.21*, **[v15.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.7.1)**
- *2021.02.19*, **[v15.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.7.0)**
- *2021.02.03*, **[v15.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.6.0)**
- *2021.02.02*, **[v15.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v15.5.2)**
- *2021.01.31*, **[v15.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.5.1)**
- *2021.01.30*, **[v15.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.5.0)**
- *2021.01.26*, **[v15.4.4](//github.com/coderaiser/cloudcmd/releases/tag/v15.4.4)**
- *2021.01.25*, **[v15.4.3](//github.com/coderaiser/cloudcmd/releases/tag/v15.4.3)**
- *2021.01.21*, **[v15.4.2](//github.com/coderaiser/cloudcmd/releases/tag/v15.4.2)**
- *2021.01.20*, **[v15.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.4.1)**
- *2021.01.19*, **[v15.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.4.0)**
- *2021.01.19*, **[v15.3.4](//github.com/coderaiser/cloudcmd/releases/tag/v15.3.4)**
- *2021.01.18*, **[v15.3.3](//github.com/coderaiser/cloudcmd/releases/tag/v15.3.3)**
- *2021.01.18*, **[v15.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v15.3.2)**
- *2021.01.17*, **[v15.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.3.1)**
- *2021.01.17*, **[v15.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.3.0)**
- *2021.01.16*, **[v15.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.2.0)**
- *2021.01.07*, **[v15.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.1.0)**
- *2021.01.05*, **[v15.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v15.0.4)**
- *2021.01.05*, **[v15.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v15.0.3)**
- *2020.12.31*, **[v15.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v15.0.2)**
- *2020.12.28*, **[v15.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v15.0.1)**
- *2020.12.28*, **[v15.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v15.0.0)**
- *2020.08.21*, **[v14.9.3](//github.com/coderaiser/cloudcmd/releases/tag/v14.9.3)**
- *2020.08.19*, **[v14.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v14.9.2)**
- *2020.08.16*, **[v14.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.9.1)**
- *2020.08.14*, **[v14.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.9.0)**
- *2020.08.14*, **[v14.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.8.0)**
- *2020.08.11*, **[v14.7.2](//github.com/coderaiser/cloudcmd/releases/tag/v14.7.2)**
- *2020.08.11*, **[v14.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.7.1)**
- *2020.08.10*, **[v14.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.7.0)**
- *2020.05.20*, **[v14.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.6.0)**
- *2020.05.06*, **[v14.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.5.1)**
- *2020.05.04*, **[v14.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.5.0)**
- *2020.04.27*, **[v14.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.4.0)**
- *2020.04.13*, **[v14.3.10](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.10)**
- *2020.04.10*, **[v14.3.9](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.9)**
- *2020.04.04*, **[v14.3.8](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.8)**
- *2020.04.03*, **[v14.3.7](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.7)**
- *2020.03.31*, **[v14.3.6](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.6)**
- *2020.03.25*, **[v14.3.5](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.5)**
- *2020.03.03*, **[v14.3.4](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.4)**
- *2020.02.23*, **[v14.3.3](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.3)**
- *2020.02.21*, **[v14.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.2)**
- *2020.02.21*, **[v14.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.1)**
- *2020.01.29*, **[v14.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.3.0)**
- *2019.12.21*, **[v14.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.2.1)**
- *2019.11.15*, **[v14.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.2.0)**
- *2019.10.16*, **[v14.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v14.1.2)**
- *2019.10.09*, **[v14.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.1.1)**
- *2019.10.02*, **[v14.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.1.0)**
- *2019.09.25*, **[v14.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v14.0.2)**
- *2019.09.25*, **[v14.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v14.0.1)**
- *2019.09.22*, **[v14.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v14.0.0)**
- *2019.09.21*, **[v13.4.2](//github.com/coderaiser/cloudcmd/releases/tag/v13.4.2)**
- *2019.09.20*, **[v13.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v13.4.1)**
- *2019.09.03*, **[v13.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v13.4.0)**
- *2019.08.28*, **[v13.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v13.3.0)**
- *2019.08.21*, **[v13.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v13.2.1)**
- *2019.08.20*, **[v13.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v13.2.0)**
- *2019.08.16*, **[v13.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v13.1.0)**
- *2019.08.14*, **[v13.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v13.0.1)**
- *2019.08.14*, **[v13.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v13.0.0)**
- *2019.08.02*, **[v12.6.3](//github.com/coderaiser/cloudcmd/releases/tag/v12.6.3)**
- *2019.06.06*, **[v12.6.2](//github.com/coderaiser/cloudcmd/releases/tag/v12.6.2)**
- *2019.06.04*, **[v12.6.1](//github.com/coderaiser/cloudcmd/releases/tag/v12.6.1)**
- *2019.05.31*, **[v12.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.6.0)**
- *2019.05.28*, **[v12.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.5.0)**
- *2019.05.27*, **[v12.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.4.0)**
- *2019.05.24*, **[v12.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v12.3.2)**
- *2019.05.24*, **[v12.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v12.3.1)**
- *2019.05.24*, **[v12.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.3.0)**
- *2019.05.13*, **[v12.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.2.0)**
- *2019.04.15*, **[v12.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.1.0)**
- *2019.04.04*, **[v12.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v12.0.2)**
- *2019.04.04*, **[v12.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v12.0.1)**
- *2019.04.01*, **[v12.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v12.0.0)**
- *2019.03.27*, **[v11.8.6](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.6)**
- *2019.02.20*, **[v11.8.5](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.5)**
- *2019.02.15*, **[v11.8.4](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.4)**
- *2018.12.04*, **[v11.8.3](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.3)**
- *2018.11.22*, **[v11.8.2](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.2)**
- *2018.11.14*, **[v11.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.1)**
- *2018.11.09*, **[v11.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.8.0)**
- *2018.11.01*, **[v11.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.7.1)**
- *2018.10.25*, **[v11.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.7.0)**
- *2018.10.23*, **[v11.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.6.0)**
- *2018.10.23*, **[v11.5.4](//github.com/coderaiser/cloudcmd/releases/tag/v11.5.4)**
- *2018.10.19*, **[v11.5.3](//github.com/coderaiser/cloudcmd/releases/tag/v11.5.3)**
- *2018.10.19*, **[v11.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v11.5.2)**
- *2018.10.17*, **[v11.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.5.1)**
- *2018.10.16*, **[v11.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.5.0)**
- *2018.10.16*, **[v11.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.4.1)**
- *2018.10.12*, **[v11.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.4.0)**
- *2018.10.12*, **[v11.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.3.1)**
- *2018.10.11*, **[v11.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.3.0)**
- *2018.10.04*, **[v11.2.3](//github.com/coderaiser/cloudcmd/releases/tag/v11.2.3)**
- *2018.09.28*, **[v11.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v11.2.2)**
- *2018.09.28*, **[v11.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v11.2.1)**
- *2018.09.28*, **[v11.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.2.0)**
- *2018.09.27*, **[v11.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.1.0)**
- *2018.09.26*, **[v11.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v11.0.0)**
- *2018.09.21*, **[v10.8.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.8.2)**
- *2018.09.20*, **[v10.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.8.1)**
- *2018.09.19*, **[v10.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.8.0)**
- *2018.09.14*, **[v10.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.7.0)**
- *2018.09.10*, **[v10.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.6.0)**
- *2018.09.08*, **[v10.5.3](//github.com/coderaiser/cloudcmd/releases/tag/v10.5.3)**
- *2018.08.25*, **[v10.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.5.2)**
- *2018.08.25*, **[v10.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.5.1)**
- *2018.08.23*, **[v10.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.5.0)**
- *2018.07.18*, **[v10.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.4.1)**
- *2018.07.17*, **[v10.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.4.0)**
- *2018.07.02*, **[v10.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.3.2)**
- *2018.06.25*, **[v10.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.3.1)**
- *2018.06.22*, **[v10.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.3.0)**
- *2018.06.21*, **[v10.2.3](//github.com/coderaiser/cloudcmd/releases/tag/v10.2.3)**
- *2018.06.15*, **[v10.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.2.2)**
- *2018.06.13*, **[v10.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.2.1)**
- *2018.06.11*, **[v10.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.2.0)**
- *2018.06.09*, **[v10.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.1.2)**
- *2018.06.08*, **[v10.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.1.1)**
- *2018.06.07*, **[v10.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.1.0)**
- *2018.06.04*, **[v10.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v10.0.3)**
- *2018.05.29*, **[v10.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v10.0.2)**
- *2018.05.29*, **[v10.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v10.0.1)**
- *2018.05.25*, **[v10.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v10.0.0)**
- *2018.05.24*, **[v9.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.6.0)**
- *2018.05.15*, **[v9.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.5.0)**
- *2018.05.08*, **[v9.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.4.0)**
- *2018.05.01*, **[v9.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v9.3.2)**
- *2018.04.30*, **[v9.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v9.3.1)**
- *2018.04.27*, **[v9.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.3.0)**
- *2018.04.25*, **[v9.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.2.0)**
- *2018.04.23*, **[v9.1.6](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.6)**
- *2018.04.19*, **[v9.1.5](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.5)**
- *2018.04.17*, **[v9.1.4](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.4)**
- *2018.04.16*, **[v9.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.3)**
- *2018.04.12*, **[v9.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.2)**
- *2018.04.10*, **[v9.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.1)**
- *2018.04.02*, **[v9.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.1.0)**
- *2018.03.30*, **[v9.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v9.0.0)**
- *2018.03.24*, **[v8.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v8.5.2)**
- *2018.03.24*, **[v8.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v8.5.1)**
- *2018.03.20*, **[v8.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.5.0)**
- *2018.03.16*, **[v8.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v8.4.1)**
- *2018.03.14*, **[v8.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.4.0)**
- *2018.03.02*, **[v8.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.3.0)**
- *2018.02.19*, **[v8.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v8.2.2)**
- *2018.01.23*, **[v8.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v8.2.1)**
- *2018.01.16*, **[v8.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.2.0)**
- *2017.12.08*, **[v8.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v8.1.3)**
- *2017.10.23*, **[v8.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v8.1.2)**
- *2017.10.19*, **[v8.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v8.1.1)**
- *2017.10.19*, **[v8.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.1.0)**
- *2017.10.13*, **[v8.0.5](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.5)**
- *2017.10.10*, **[v8.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.4)**
- *2017.10.06*, **[v8.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.3)**
- *2017.10.06*, **[v8.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.2)**
- *2017.10.02*, **[v8.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.1)**
- *2017.10.02*, **[v8.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v8.0.0)**
- *2017.09.29*, **[v7.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.9.0)**
- *2017.09.25*, **[v7.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.8.0)**
- *2017.09.22*, **[v7.7.3](//github.com/coderaiser/cloudcmd/releases/tag/v7.7.3)**
- *2017.09.22*, **[v7.7.2](//github.com/coderaiser/cloudcmd/releases/tag/v7.7.2)**
- *2017.09.18*, **[v7.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.7.1)**
- *2017.09.12*, **[v7.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.7.0)**
- *2017.09.11*, **[v7.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.6.0)**
- *2017.09.08*, **[v7.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v7.5.2)**
- *2017.09.08*, **[v7.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.5.1)**
- *2017.09.08*, **[v7.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.5.0)**
- *2017.09.04*, **[v7.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.4.0)**
- *2017.08.29*, **[v7.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v7.3.2)**
- *2017.08.14*, **[v7.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.3.1)**
- *2017.08.14*, **[v7.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.3.0)**
- *2017.08.11*, **[v7.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v7.2.2)**
- *2017.07.31*, **[v7.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.2.1)**
- *2017.07.28*, **[v7.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.2.0)**
- *2017.07.27*, **[v7.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.1.1)**
- *2017.07.27*, **[v7.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.1.0)**
- *2017.07.14*, **[v7.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v7.0.2)**
- *2017.07.12*, **[v7.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v7.0.1)**
- *2017.07.12*, **[v7.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v7.0.0)**
- *2017.07.10*, **[v6.15.5](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.5)**
- *2017.07.10*, **[v6.15.4](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.4)**
- *2017.06.26*, **[v6.15.3](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.3)**
- *2017.06.22*, **[v6.15.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.2)**
- *2017.06.14*, **[v6.15.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.1)**
- *2017.06.06*, **[v6.15.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.15.0)**
- *2017.05.25*, **[v6.14.4](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.4)**
- *2017.05.22*, **[v6.14.4](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.4)**
- *2017.05.22*, **[v6.14.4](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.3)**
- *2017.05.18*, **[v6.14.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.2)**
- *2017.05.18*, **[v6.14.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.1)**
- *2017.05.17*, **[v6.14.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.14.0)**
- *2017.05.15*, **[v6.13.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.13.0)**
- *2017.05.12*, **[v6.12.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.12.0)**
- *2017.05.10*, **[v6.11.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.11.0)**
- *2017.04.25*, **[v6.10.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.10.1)**
- *2017.04.24*, **[v6.10.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.10.0)**
- *2017.04.18*, **[v6.9.3](//github.com/coderaiser/cloudcmd/releases/tag/v6.9.3)**
- *2017.04.13*, **[v6.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.9.2)**
- *2017.04.12*, **[v6.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.9.1)**
- *2017.03.23*, **[v6.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.9.0)**
- *2017.03.21*, **[v6.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.8.1)**
- *2017.03.06*, **[v6.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.8.0)**
- *2017.03.04*, **[v6.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.7.0)**
- *2017.02.24*, **[v6.6.3](//github.com/coderaiser/cloudcmd/releases/tag/v6.6.3)**
- *2017.02.24*, **[v6.6.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.6.2)**
- *2017.02.24*, **[v6.6.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.6.1)**
- *2017.02.22*, **[v6.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.6.0)**
- *2017.02.21*, **[v6.5.6](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.6)**
- *2017.02.21*, **[v6.5.5](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.5)**
- *2017.02.17*, **[v6.5.4](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.4)**
- *2017.02.17*, **[v6.5.3](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.3)**
- *2017.02.15*, **[v6.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.2)**
- *2017.02.14*, **[v6.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.1)**
- *2017.02.14*, **[v6.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.5.0)**
- *2017.02.06*, **[v6.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.4.0)**
- *2017.02.02*, **[v6.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.3.1)**
- *2017.01.27*, **[v6.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.3.0)**
- *2017.01.26*, **[v6.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.2.2)**
- *2017.01.24*, **[v6.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.2.1)**
- *2017.01.24*, **[v6.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.2.0)**
- *2017.01.20*, **[v6.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.1.0)**
- *2017.01.17*, **[v6.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v6.0.3)**
- *2017.01.08*, **[v6.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v6.0.2)**
- *2017.01.06*, **[v6.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v6.0.1)**
- *2016.12.29*, **[v6.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v6.0.0)**
- *2016.12.27*, **[v5.13.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.13.0)**
- *2016.12.23*, **[v5.12.4](//github.com/coderaiser/cloudcmd/releases/tag/v5.12.4)**
- *2016.12.23*, **[v5.12.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.12.3)**
- *2016.12.19*, **[v5.12.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.12.2)**
- *2016.12.19*, **[v5.12.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.12.1)**
- *2016.12.16*, **[v5.12.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.12.0)**
- *2016.12.05*, **[v5.11.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.11.1)**
- *2016.12.01*, **[v5.11.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.11.0)**
- *2016.12.01*, **[v5.10.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.10.2)**
- *2016.11.22*, **[v5.10.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.10.1)**
- *2016.11.18*, **[v5.10.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.10.0)**
- *2016.11.10*, **[v5.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.9.1)**
- *2016.11.10*, **[v5.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.9.0)**
- *2016.11.09*, **[v5.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.8.0)**
- *2016.11.06*, **[v5.7.6](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.6)**
- *2016.11.06*, **[v5.7.5](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.5)**
- *2016.10.27*, **[v5.7.4](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.4)**
- *2016.10.27*, **[v5.7.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.3)**
- *2016.10.24*, **[v5.7.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.2)**
- *2016.10.24*, **[v5.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.1)**
- *2016.10.18*, **[v5.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.7.0)**
- *2016.09.22*, **[v5.6.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.6.2)**
- *2016.09.06*, **[v5.6.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.6.1)**
- *2016.07.19*, **[v5.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.6.0)**
- *2016.06.29*, **[v5.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.5.1)**
- *2016.06.15*, **[v5.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.5.0)**
- *2016.06.10*, **[v5.4.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.4.3)**
- *2016.06.09*, **[v5.4.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.4.2)**
- *2016.05.25*, **[v5.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.4.1)**
- *2016.05.15*, **[v5.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.4.0)**
- *2016.05.11*, **[v5.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.3.2)**
- *2016.03.28*, **[v5.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.3.1)**
- *2016.03.28*, **[v5.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.3.0)**
- *2016.03.18*, **[v5.2.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.2.3)**
- *2016.03.10*, **[v5.2.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.2.2)**
- *2016.03.07*, **[v5.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.2.1)**
- *2016.03.05*, **[v5.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.2.0)**
- *2016.02.26*, **[v5.1.5](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.5)**
- *2016.02.25*, **[v5.1.4](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.4)**
- *2016.02.24*, **[v5.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.3)**
- *2016.02.21*, **[v5.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.2)**
- *2016.02.21*, **[v5.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.1)**
- *2016.02.20*, **[v5.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.1.0)**
- *2016.02.13*, **[v5.0.15](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.15)**
- *2016.02.10*, **[v5.0.14](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.14)**
- *2016.02.10*, **[v5.0.13](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.13)**
- *2016.02.10*, **[v5.0.12](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.12)**
- *2016.02.06*, **[v5.0.11](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.11)**
- *2016.02.04*, **[v5.0.10](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.10)**
- *2016.02.02*, **[v5.0.9](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.9)**
- *2016.02.01*, **[v5.0.8](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.8)**
- *2016.01.20*, **[v5.0.7](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.7)**
- *2016.01.15*, **[v5.0.6](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.6)**
- *2016.01.11*, **[v5.0.5](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.5)**
- *2015.12.26*, **[v5.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.4)**
- *2015.12.08*, **[v5.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.3)**
- *2015.12.01*, **[v5.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.2)**
- *2015.11.15*, **[v5.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.1)**
- *2015.11.15*, **[v5.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v5.0.0)**
- *2015.11.11*, **[v4.7.7](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.7)**
- *2015.11.06*, **[v4.7.6](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.6)**
- *2015.10.29*, **[v4.7.5](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.5)**
- *2015.10.27*, **[v4.7.4](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.4)**
- *2015.10.24*, **[v4.7.3](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.3)**
- *2015.10.14*, **[v4.7.2](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.2)**
- *2015.10.14*, **[v4.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.1)**
- *2015.10.05*, **[v4.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.7.0)**
- *2015.09.28*, **[v4.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.6.0)**
- *2015.09.27*, **[v4.5.7](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.7)**
- *2015.09.24*, **[v4.5.6](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.6)**
- *2015.09.23*, **[v4.5.5](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.5)**
- *2015.09.22*, **[v4.5.4](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.4)**
- *2015.09.16*, **[v4.5.3](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.3)**
- *2015.09.03*, **[v4.5.2](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.2)**
- *2015.08.28*, **[v4.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.1)**
- *2015.08.26*, **[v4.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.5.0)**
- *2015.08.25*, **[v4.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.4.0)**
- *2015.08.21*, **[v4.3.5](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.5)**
- *2015.08.19*, **[v4.3.4](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.4)**
- *2015.08.17*, **[v4.3.3](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.3)**
- *2015.08.17*, **[v4.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.2)**
- *2015.08.13*, **[v4.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.1)**
- *2015.08.11*, **[v4.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.3.0)**
- *2015.07.24*, **[v4.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.2.0)**
- *2015.07.23*, **[v4.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v4.1.2)**
- *2015.07.23*, **[v4.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v4.1.1)**
- *2015.07.21*, **[v4.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.1.0)**
- *2015.07.13*, **[v4.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v4.0.0)**
- *2015.07.09*, **[v3.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v3.8.1)**
- *2015.07.06*, **[v3.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.8.0)**
- *2015.07.04*, **[v3.7.2](//github.com/coderaiser/cloudcmd/releases/tag/v3.7.2)**
- *2015.07.04*, **[v3.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v3.7.1)**
- *2015.07.03*, **[v3.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.7.0)**
- *2015.07.01*, **[v3.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.6.0)**
- *2015.06.27*, **[v3.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.5.0)**
- *2015.06.22*, **[v3.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.4.0)**
- *2015.06.20*, **[v3.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.3.0)**
- *2015.06.12*, **[v3.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.2.0)**
- *2015.06.11*, **[v3.1.4](//github.com/coderaiser/cloudcmd/releases/tag/v3.1.4)**
- *2015.06.11*, **[v3.1.3](//github.com/coderaiser/cloudcmd/releases/tag/v3.1.3)**
- *2015.06.10*, **[v3.1.2](//github.com/coderaiser/cloudcmd/releases/tag/v3.1.2)**
- *2015.06.09*, **[v3.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v3.1.1)**
- *2015.06.09*, **[v3.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.1.0)**
- *2015.06.04*, **[v3.0.4](//github.com/coderaiser/cloudcmd/releases/tag/v3.0.4)**
- *2015.06.02*, **[v3.0.3](//github.com/coderaiser/cloudcmd/releases/tag/v3.0.3)**
- *2015.05.31*, **[v3.0.2](//github.com/coderaiser/cloudcmd/releases/tag/v3.0.2)**
- *2015.05.29*, **[v3.0.1](//github.com/coderaiser/cloudcmd/releases/tag/v3.0.1)**
- *2015.05.28*, **[v3.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v3.0.0)**
- *2015.05.22*, **[v2.9.3](//github.com/coderaiser/cloudcmd/releases/tag/v2.9.3)**
- *2015.05.22*, **[v2.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v2.9.2)**
- *2015.05.19*, **[v2.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.9.1)**
- *2015.05.15*, **[v2.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.9.0)**
- *2015.05.14*, **[v2.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.8.0)**
- *2015.04.24*, **[v2.7.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.7.1)**
- *2015.04.24*, **[v2.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.7.0)**
- *2015.04.17*, **[v2.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.6.0)**
- *2015.04.14*, **[v2.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.5.1)**
- *2015.04.09*, **[v2.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.5.0)**
- *2015.04.03*, **[v2.4.2](//github.com/coderaiser/cloudcmd/releases/tag/v2.4.2)**
- *2015.03.28*, **[v2.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.4.1)**
- *2015.03.28*, **[v2.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.4.0)**
- *2015.03.26*, **[v2.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.3.1)**
- *2015.03.26*, **[v2.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.3.0)**
- *2015.03.19*, **[v2.2.1](//github.com/coderaiser/cloudcmd/releases/tag/v2.2.1)**
- *2015.03.13*, **[v2.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.2.0)**
- *2015.02.02*, **[v2.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.1.0)**
- *2014.12.09*, **[v2.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v2.0.0)**
- *2014.11.21*, **[v1.5.1](//github.com/coderaiser/cloudcmd/releases/tag/v1.5.1)**
- *2014.11.19*, **[v1.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.5.0)**
- *2014.11.05*, **[v1.4.1](//github.com/coderaiser/cloudcmd/releases/tag/v1.4.1)**
- *2014.10.28*, **[v1.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.4.0)**
- *2014.10.02*, **[v1.3.2](//github.com/coderaiser/cloudcmd/releases/tag/v1.3.2)**
- *2014.09.22*, **[v1.3.1](//github.com/coderaiser/cloudcmd/releases/tag/v1.3.1)**
- *2014.09.18*, **[v1.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.3.0)**
- *2014.08.29*, **[v1.2.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.2.0)**
- *2014.07.18*, **[v1.1.1](//github.com/coderaiser/cloudcmd/releases/tag/v1.1.1)**
- *2014.07.10*, **[v1.1.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.1.0)**
- *2014.07.03*, **[v1.0.0](//github.com/coderaiser/cloudcmd/releases/tag/v1.0.0)**
- *2014.06.16*, **[v0.9.2](//github.com/coderaiser/cloudcmd/releases/tag/v0.9.2)**
- *2014.06.11*, **[v0.9.1](//github.com/coderaiser/cloudcmd/releases/tag/v0.9.1)**
- *2014.06.10*, **[v0.9.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.9.0)**
- *2014.04.28*, **[v0.8.4](//github.com/coderaiser/cloudcmd/releases/tag/v0.8.4)**
- *2014.03.19*, **[v0.8.3](//github.com/coderaiser/cloudcmd/releases/tag/v0.8.3)**
- *2014.03.03*, **[v0.8.2](//github.com/coderaiser/cloudcmd/releases/tag/v0.8.2)**
- *2014.02.13*, **[v0.8.1](//github.com/coderaiser/cloudcmd/releases/tag/v0.8.1)**
- *2014.02.13*, **[v0.8.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.8.0)**
- *2013.12.09*, **[v0.7.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.7.0)**
- *2013.11.08*, **[v0.6.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.6.0)**
- *2013.10.17*, **[v0.5.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.5.0)**
- *2013.09.27*, **[v0.4.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.4.0)**
- *2013.08.01*, **[v0.3.0](//github.com/coderaiser/cloudcmd/releases/tag/v0.3.0)**
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
- [Олена Заліток](https://www.linkedin.com/in/ozalitok-ux-ui/ "Олена Заліток") за **logo** та **favicon**.
- [TarZak](https://github.com/tarzak "TarZak")
    - Російський та український переклади;
    - налаштування: шаблон та стилі
