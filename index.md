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
---

Cloud Commander 1.1.0
===============
###[Головна][MainURL] [Блог][BlogURL] Наживо(![JitSu][JitSu_LIVE_IMG] [JitSu][JitSuURL], ![Heroku][Heroku_LIVE_IMG] [Heroku][HerokuURL])
[NPM_INFO_IMG]:             https://nodei.co/npm/cloudcmd.png?downloads=true&&stars "npm install cloudcmd"
[MainURL]:                  http://cloudcmd.io "Головна"
[BlogURL]:                  http://blog.cloudcmd.io "Блог"
[JitSuURL]:                 http://cloudcmd.jit.su "JitSu"
[HerokuURL]:                http://cloudcmd.herokuapp.com/ "Heroku"
[JitSu_LIVE_IMG]:           https://status-ok.cloudcmd.io/host/cloudcmd.jit.su/img/txt.png "JitSu"
[HEROKU_LIVE_IMG]:          https://status-ok.cloudcmd.io/host/cloudcmd.herokuapp.com/img/txt.png "Heroku"

**Cloud Commander** - двопанельний веб файл менеджер з консоллю та редактором. Допоможе вам керувати сервером та працювати з файлами, папками і програмами в браузері на будь-якому комп'ютері, смартфоні або планшеті.

![Cloud Commander](http://cloudcmd.io/img/logo/cloudcmd.png "Cloud Commander")

Переваги
---------------
- Відкритий код (**MIT License**).
- Має дві класичні панелі.
- Можливість **авторизації**.
- Клієнт працює в веб браузері.
- Сервер працює під **Windows**, **Linux** та **Mac OS**.
- Може використовуватись локально або віддалено.
- Підлаштовується під розмір екрану.
- **Редактор** з підтримкою **підсвітки синтаксису** більш ніж для 110 мов.
- **Консоль** з підтримкою стандартної командної строки ОС.
- Написаний на **JavaScript/Node.js**.
 
Встановлення
---------------

**Cloud Commander** встановлюється дуже просто:

- встановити [node.js](http://nodejs.org/ "node.js").
- встановити ```cloudcmd``` через npm за допомогою однієї простої команди.

![NPM_INFO][NPM_INFO_IMG]

Запуск
---------------
Для запуску **Cloud Commander** потрібна лише одна команда:
    
    node cloudcmd

або, при глобальному встановленні:

    cloudcmd

Cloud Commander читає інформацію порта з файлу налаштувань `json/config.json` і запускає сервер на стандартному порту (`8000`), якщо змінних оточнення з іменами `cloud9`, `cloudfoundry` та `nodester` не існує.
Для початку роботи просто наберіть в броузері

    http://127.0.0.1:8000
    
Оновлення
---------------
**Cloud Commander** оновлюється часто.

Оновлення проходить автоматично, але можна також виконувати вручну.
Якщо Ви клонували репозиторій, Ви можете отримати останні зміни командою:

 git pull

Якщо ви встановили Cloud Commander за допомогою `npm`, просто перевстановіть його:

 npm i cloudcmd -g

Після цього почистіть кеш вашого браузеру, перезапустіть Cloud Commander та оновіть сторінку.

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
| `F7`                  | нова папка
| `Shift + F7`          | новий файл
| `Shift + Delete`      | знищити без підтвердження
| `F8`, `Delete`        | знищити обраний файл
| `F9`                  | меню
| `F10`                 | налаштування
| `(*)`                 | виділити/зняти виділення з усього
| `(+)`                 | розширити виділення
| `(-)`                 | звузити виділення
| `Ctrl + r`            | оновити
| `Ctrl + d`            | очистити локальний кеш, що містить вміст папки
| `Alt  + q`            | вимкнути прив'язку клавіш
| `Alt  + s`            | відновити усі прив'язки клавіші
| `Ctrl + a`            | виділити усі файли на панелі
| `Up`, `Down`, `Enter` | пересування файловою систему
| `Ctrl + \`            | перейти до кореневого каталогу
| `Tab`                 | переміщення між панелями
| `Page Up`             | вгору на одну сторінку
| `Page Down`           | вниз на одну сторінку 
| `Home`                | на початок списку 
| `End`                 | в кінець списку
| `Space`               | обрати поточнний файл (і отримати розмір папки)
| `Insert`              | обрати поточнний файл (і перейти до наступного)
| `Shift + F10`         | контекстне меню
| `~`                   | консоль
| `Ctrl + Click`        | відкрити файл в новій вкладці

Редактор
---------------
![Edit](http://cloudcmd.io/img/screen/edit.png "Edit")

###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F4`                  | відкрити
| `Ctrl + s`            | зберегти
| `Ctrl + f`            | пошук
| `Ctrl + f + f`        | заміна
| `Ctrl + g`            | перейти до строки
| `Esc`                 | закрити

Детальніше [Гарячі клавіші Ace](https://github.com/ajaxorg/ace/wiki/Default-Keyboard-Shortcuts "Гарячі клавіші Ace").

Консоль
---------------
![Консоль](http://cloudcmd.io/img/screen/console.png "Консоль")

###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `~`                   | відкрити
| `Ctrl + p`            | вставити шлях поточної папки
| `Ctrl + z`            | скасувати поточний рядок
| `Ctrl + l`            | очистити
| `Esc`                 | закрити

Налаштування
---------------
![Налаштування](http://cloudcmd.io/img/screen/config.png "Налаштування")

###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F10`                 | відкрити
| `Esc`                 | закрити

Меню
---------------
![Menu](http://cloudcmd.io/img/screen/menu.png "Меню")
Натискання на праву клавішу мишки, викликає меню з наступними пунктами:

- Перегляд
- Редагування
- Змінити назву
- Знищити
- Zip файл
- UnZip файл
- Обрати все
- Вивантажити до (Dropbox, Github, GDrive)
- Завантажити
- Новий (Файл, Папка, з хмари)
 
###Гарячі клавіші
|Клавіша                |Дія
|:----------------------|:--------------------------------------------
| `F9`                  | відкрити
| `Esc`                 | закрити

Налаштування
---------------
Всі головні налаштування можна встановити в `json/config.json`.

```js
{
    "auth"              : false,     /* дозволити http авторизацію                                  */
    "username"          : "root",    /* ім'я користувача для авторизації                            */
    "password"          : "toor",    /* хеш пароль в sha-1 для авторизації                          */
    "appCache"          : false,     /* кешувати файли для оффлайнового використання                */
    "analytics"         : true,      /* підтримка google analytics                                  */
    "diff"              : false,     /* при збереженні - відсилає патч, а не повний файл            */
    "zip"               : false,     /* zip текст пере посиланням / unzip перед збереженням         */
    "notifications"     : false,     /* показувати сповіщення, коли вкладка не активна              */
    "localStorage"      : true,      /* кешування вмісту папки                                      */
    "minify"            : true,      /* мініфікація js, css, html та зображень                      */
    "cache"             : true,      /* додати контроль кешу                                        */
    "online"            : true,      /* загрузити файли js з cdn або Local path                     */
    "logs"              : false,     /* виводити в логи чи в консоль                                */
    "showKeysPanel"     : true,      /* показати класичну панель з кнопками функціональних клавіш   */
    "server"            : true,      /* режим сервера чи тестування                                 */
    "socket"            : true       /* увімкнути web сокети                                        */
    "port"              : 8000,      /* http порт                                                   */
    "sslPort"           : 443,       /* https порт                                                  */
    "ip"                : null,      /* ip чи null(за замовчуванням)                                */
    "ssl"               : false      /* використовувати https?                                      */
    "rest"              : true       /* увімкнути решту інтерфейса                                  */
}
```

Якщо ви змінили **config** і хочете продовжувати оновлюватись за допомогою git,
вам потрібно виконати наступну команду в кореневій директорії **Cloud Commander**:

```
git update-index --assume-unchanged json/config.json
```

Щоб повернутися до відстежування:

```
git update-index --no-assume-unchanged json/config.json
```

Сервер
---------------
Зазвичай процеси, що запущено правами не root не можуть прослуховувати порти нижче ніж 1024.
В любому випадку, я раджу Вам запускати Cloud Commander не під рутом. Як це зробити?!
Існує декілька простих і швидких шляхів. Один з них - просування портів через iptables.

###Iptables
Просто запустіть `shell/addtables.sh` для стандартних опцій.

```sh
iptables -t nat -L # look rules before
iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 8000
iptables -t nat -A PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 4430
iptables -t nat -L # look rules after
```

Ви маєте побачити щось назразок ( **8000** та **4430** мають бути в config як **port** і **sslPort** )

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

Якщо ви бажаєте додати **ssl**, додайте декілька рядків в розділ серверу:

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

Для запуску Cloud Commander в якості daemon в Linux встановіть **log** в "істину" в config-файлі і
зробіть щось на зразок:
    
    nohup node cloudcmd

Список додаткових модулів
---------------
Щоб розширити функціонал файлового менеджера, використовуются такі модулі:

- [Ace]                     [AceURL]
- [Diff-Match-Patch]        [Diff-Match-PatchURL]
- [Minify]                  [MinifyURL]
- [FancyBox]                [FancyBoxURL]
- [jQuery-contextMenu]      [jQuery-contextMenuURL]
- [jq-console]              [jq-consoleURL]
- [github]                  [githubURL]
- [dropbox-js]              [dropbox-jsURL]
- [jquery]                  [jqueryURL]
- [socket.io]               [socketIOURL]
- [http-auth]               [httpAuthURL]
- [rimraf]                  [rimrafURL]
- [mkdirp]                  [mkdirpURL]

[AceURL]:                   http://ace.ajax.org/ "Ace"
[Diff-Match-PatchURL]:      https://code.google.com/p/google-diff-match-patch/ "Diff-Match-Patch"
[MinifyURL]:                http://coderaiser.github.io/minify "Minify"
[FancyBoxURL]:              //github.com/fancyapps/fancyBox "FancyBox"
[jQuery-contextMenuURL]:    //github.com/medialize/jQuery-contextMenu "jQuery-contextMenu"
[jq-consoleURL]:            //github.com/replit/jq-console "jq-console"
[githubURL]:                //github.com/michael/github "github"
[dropbox-jsURL]:            //github.com/dropbox/dropbox-js "dropbox-js"
[jqueryURL]:                //jquery.com
[socketIOURL]:              http://socket.io
[httpAuthURL]:              //github.com/gevorg/http-auth
[rimrafURL]:                //github.com/isaacs/rimraf "rimraf"
[mkdirpURL]:                //github.com/substack/node-mkdirp

Долучитися до проекту
---------------
Якщо ви хочете долучитися до проекту — відправте pull запит в dev гілку.
Отримання dev версії **Cloud Commander**:

    git clone git://github.com/coderaiser/cloudcmd.git
    cd cloudcmd && git checkout dev

Можливо, вам знадобиться dev версія Minify,
щоб отримати її, вам потрібно ввести декілька команд:

    cd node_modules
    rm -rf minify
    git clone git://github.com/coderaiser/minify
    git checkout dev

Історія версій
---------------
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
    - налаштування: [шаблон](html/config.html) та [стилі](css/config.css);
