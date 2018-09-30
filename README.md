<h1 align="center">
<a href="https://lectrum.io" target="_blank" rel="noopener noreferrer"> <img src="./static/favicon/favicon-woodsmoke.svg" alt="Lectrum favicon" width="25" /></a> FAQ</h1>

<br>



<table align="center">
    <tbody>
        <tr>
            <td>
                <h3 align="center">👋🏼 Привет и добро пожаловать!</h3>
                <p>
                    🤔&nbsp;Здесь ты найдешь ответы на часто задаваемые вопросы.
                </p>
                <br>
                <p>👨🏽‍🔬&nbsp;Ответы на вопросы, а также инструкции и ссылки на полезные гайды можно найти ниже в README.md этого репозитория.</p>
            </td>
        </tr>
    <tbody>
</table>

<br>

## 📜 Содержание
<!-- TOC -->

- [🌏 Настройка окружения](#-Настройка-окружения)
    - [Какие операционные системы поддерживаются обучающими проектами компании Lectrum?](#Какие-операционные-системы-поддерживаются-обучающими-проектами-компании-lectrum)
    - [Как установить Node.js?](#Как-установить-nodejs)
    - [Что такое nvm?](#Что-такое-nvm)
    - [Зачем мне устанавливать Node.js именно через nvm?](#Зачем-мне-устанавливать-nodejs-именно-через-nvm)
    - [Как установить или обновить Git?](#Как-установить-или-обновить-git)
    - [Как обновить Node.js?](#Как-обновить-nodejs)
    - [Я пользователь Windows. Как настроить терминал для удобной работы?](#Я-пользователь-windows-Как-настроить-терминал-для-удобной-работы)
    - [Какой редактор кода мне использовать?](#Какой-редактор-кода-мне-использовать)
    - [Что такое Yeoman?](#Что-такое-yeoman)
    - [Нужно ли запускать `npm audit fix` после установки зависимостей?](#Нужно-ли-запускать-npm-audit-fix-после-установки-зависимостей)
    - [Как убрать предупреждение experimentalDecorators из VSCode?](#Как-убрать-предупреждение-experimentaldecorators-из-vscode)
    - [Как настроить PostCSS в VSCode?](#Как-настроить-postcss-в-vscode)
    - [Как исправить ошибку, связанную с нехваткой памяти при установке PhantomJS для пользователей Ubuntu?](#Как-исправить-ошибку-связанную-с-нехваткой-памяти-при-установке-phantomjs-для-пользователей-ubuntu)
- [🏎 Запуск и работа с проектом](#-Запуск-и-работа-с-проектом)
    - [У меня не запускается проект. Что делать?](#У-меня-не-запускается-проект-Что-делать)
    - [Как остановить запущенный командой npm run start (или yarn start) проект?](#Как-остановить-запущенный-командой-npm-run-start-или-yarn-start-проект)
- [🥊 npm и yarn](#-npm-и-yarn)
    - [В чём разница между npm и yarn?](#В-чём-разница-между-npm-и-yarn)
    - [Что лучше: npm или yarn?](#Что-лучше-npm-или-yarn)
- [✏️ Качество кода: настройка редакторов и IDE](#️-Качество-кода-настройка-редакторов-и-ide)
    - [Почему редактор подсвечивает мой код?](#Почему-редактор-подсвечивает-мой-код)
    - [Что такое линтер?](#Что-такое-линтер)
    - [Что такое `Prettier`?](#Что-такое-prettier)
    - [Как сделать, чтобы `Prettier` и `ESLint` работали вместе?](#Как-сделать-чтобы-prettier-и-eslint-работали-вместе)

<!-- /TOC -->

<br>

## 🌏 Настройка окружения

#### Какие операционные системы поддерживаются обучающими проектами компании Lectrum?

Поддерживаемые операционные системы:
+ macOS: **`Mojave`**, **`High Sierra`**;
+ Ubuntu: **`16.04.01`**, **`18.04.01`**;
+ Windows: **`10`**.

<br>

#### Как установить Node.js?
Есть несколько способов:
+ Для пользователей MacOS и Ubuntu лучше установить [nvm](https://github.com/creationix/nvm#installation);
+ Для пользователей Windows можно [скачать установщик с официального сайта](https://nodejs.org/en/).

<br>

#### Что такое nvm?
[nvm](https://github.com/creationix/nvm) — это сокращение от Node Version Manager. То есть nvm — это **`менеджер версий Node.js`**.
С помощью nvm на одном компьютере можно держать сразу несколько разных версий Node.js, и легко переключатся между ними. Каждая версия находится в изолированном и независимом окружении, что очень удобно — одна версия Node.js никогда ничего не сломает в другой версии.

<br>

#### Зачем мне устанавливать Node.js именно через nvm?
Дело в том, что `nvm` — это удобный инструмент для работы в Node.js. Но кроме того, для правильной работы наших проектов необходимо исправить права для `npm` на твоём компьютере (чтобы можно было писать `npm install ...` без `sudo`). Если ты по какой-то причине не хочешь устанавливать `nvm` — не проблема. Главное исправить права для `npm`. `nvm` исправляет права для `npm` автоматически. Но это можно сделать и самостоятельно, [следуя этому гайду](https://docs.npmjs.com/getting-started/fixing-npm-permissions).

<br>

#### Как установить или обновить Git?
[Скачай с официального сайта](https://git-scm.com/download/) и установи последнюю версию Git.

<br>

#### Как обновить Node.js?
Есть несколько способов, в зависимости от того, как ты устанавливал Node.js.
+ `Первый`: если ты установил Node.js установщиком с сайта, то обновить тоже нужно с помощью [установщика последней версии](https://nodejs.org/en/).
+ `Второй`: если ты установил Node.js [через `nvm`](https://github.com/creationix/nvm), то обновить тоже нужно с помощью команды `nvm install --lts --latest-npm`.

<br>

#### Я пользователь Windows. Как настроить терминал для удобной работы?
Есть несколько вариантов. Список составлен начиная из лучшего варианта, заканчивая самым обычным:
+ В современной веб-разработке наиболее удобным является UNIX-окружение. Чтобы настроить его [установи Ubuntu shell](https://remontka.pro/linux-bash-shell-windows-10/). Это позволит тебе работать на Windows в [UNIX-окружении Ubuntu](https://www.microsoft.com/en-us/p/ubuntu/9nblggh4msv6).
+ Рекомендуем также рассмотреть [терминал CMDER](http://cmder.net/), альтернативу обычному терминалу `Windows Command Prompt (CMD)`. Например, в CMDER есть встроенный git, а интерфейс выглядит куда приятней, чем в `Command Prompt (CMD)`.
+ Если никакой из вышеперечисленых вариантов не подойдёт, используй встроенный в Windows терминал `Command Prompt (CMD)`.

<br>

#### Какой редактор кода мне использовать?
Мы рекомендуем использовать [VSCode](https://code.visualstudio.com/). Этот редактор доступен для всех основных операционных систем. А также он быстрый (быстрее [Atom](https://atom.io/)), активно развивается, а также обладает богатой базой удобных расширений. Вот список самых полезных:
+ [Babel syntax highlightin](https://marketplace.visualstudio.com/items?itemName=mgmcdermott.vscode-language-babel): эта подсветка является самой современной, поддерживает все фичи JavaScript а также синтаксис JSX React;
+ [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): лучший на сегодняшний день [линтер](#-Вопрос-что-такое-линтер) JavaScript-кода для VSCode;
+ [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode): встроенный в VSCode Prettier. С его помощью можно удобно форматировать JavaScript-код нажатием сочетания клавиш. Очень удобно;
+ [Auto rename tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag): этот плагин будет автоматически обновлять имя парного тега разметки;
+ [File icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons): добавляет красивые иконки для всевозможных типов файлов в сайдбаре.

Также можно установить полный список расширений, который используется компанией Lectrum одной командой в терминале:

```bash
code --install-extension aaron-bond.better-comments
code --install-extension AlanWalk.markdown-toc
code --install-extension alefragnani.project-manager
code --install-extension asvetliakov.snapshot-tools
code --install-extension christian-kohler.npm-intellisense
code --install-extension christian-kohler.path-intellisense
code --install-extension CoenraadS.bracket-pair-colorizer
code --install-extension dbaeumer.vscode-eslint
code --install-extension eamodio.gitlens
code --install-extension esbenp.prettier-vscode
code --install-extension formulahendry.auto-rename-tag
code --install-extension formulahendry.code-runner
code --install-extension gaearon.subliminal
code --install-extension jasonnutter.search-node-modules
code --install-extension mgmcdermott.vscode-language-babel
code --install-extension naumovs.color-highlight
code --install-extension pnp.polacode
code --install-extension redhat.vscode-yaml
code --install-extension robertohuertasm.vscode-icons
code --install-extension sdras.night-owl
code --install-extension Shan.code-settings-sync
code --install-extension shinnn.stylelint
code --install-extension sldobri.daily
code --install-extension streetsidesoftware.code-spell-checker
code --install-extension streetsidesoftware.code-spell-checker-russian
code --install-extension tomphilbin.gruvbox-themes
code --install-extension Tyriar.sort-lines
code --install-extension yogipatel.solarized-light-no-bold
```

> P.S.: перед запуском этого набора команд проверь, есть ли в твоём терминале возможность вызывать Visual Studio Code из терминала с помощью **`code`**. Для этого выполни команду **`code`** в терминале. Команда должна открыть редактор VSCode. Если этого не произошло пройди инструкцию: [Mac](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line), [Windows](https://code.visualstudio.com/docs/editor/command-line#_launching-from-command-line)

<br>

#### Что такое Yeoman?
[Yeoman](http://yeoman.io/) — это инструмент для автоматического создания и обновления проектов. С его помощью можно развернуть проект одной командой, что очень удобно.

<br>

#### Нужно ли запускать `npm audit fix` после установки зависимостей?
Нет, не нужно.

<br>

#### Как убрать предупреждение experimentalDecorators из VSCode?
Пройди инструкцию [из этого гайда](https://ihatetomatoes.net/how-to-remove-experimentaldecorators-warning-in-vscode/).

<br>

#### Как настроить PostCSS в VSCode?
Для интеграции синтаксиса PostCSS [используй этот плагин](https://marketplace.visualstudio.com/items?itemName=ricard.PostCSS).

<br>


#### Как исправить ошибку, связанную с нехваткой памяти при установке PhantomJS для пользователей Ubuntu
О наличии такой ошибки может говорить следующее сообщение в консоли:

```bash
Phantom installation failed { Error: spawn ENOMEM
```

Для решения этой проблемы выполни следующие команды в консоли:


+ sudo fallocate -l 4G /swapfile 
+ sudo chmod 600 /swapfile
+ sudo mkswap /swapfile
+ sudo swapon /swapfile
+ echo "/swapfile none swap sw 0 0" | sudo tee -a /etc/fstab

Затем удали `node_modules`: **`rm -rf node_modules`**. И установи зависимости заново: **`npm install`**.


<br>

---

<br>

## 🏎 Запуск и работа с проектом

#### У меня не запускается проект. Что делать?
Есть несколько решений.

1. Посмотри консоль на наличие ошибок;
2. Прочитай текст ошибки. Чаще всего, текст ошибки сам по себе объясняет её причину.
    + Самая частая ошибка: `Error: listen EADDRINUSE 0.0.0.0:3000`. Давай разберёмся как её решить. Читаем:
        + Первое слово — `Error`, говорит о том, что это ошибка;
        + Второе слово — `listen`, говорит о том, что ошибка связана с процессом «прослушивания»;
        + Далее — `EADDRINUSE 0.0.0.0:3000`, первая часть (буквы) — это описание ошибки, вторая часть (цифры) — адрес в формате хост:порт;
        + `EADDRINUSE` — это аббревиатура. Пу сути её можно разгадать путем обычной логики:
            + `E` — означает Error, ошибка;
            + `ADDR` — сокращение от address, адрес;
            + `INUSE` — сокращение in use — в использовании.
        + В итоге можно сделать вывод, что адрес `0.0.0.0:3000` чем-то используется. Webpack поднимает проект именно на этом адресе. Этот адрес уже занят каким-то процессом, поэтому — возникает ошибка;
        + **`Решение`**:
            + Найди, какие процессы твоего компьютера используют данный адрес, и выключи их;
            + Если не можешь найти их через терминал — перегрузи компьютер.

<br>

#### Как остановить запущенный командой npm run start (или yarn start) проект?
В терминале нажми сочетание клавиш `CTRL` + `C`.

<br>

---

<br>

## 🥊 npm и yarn

#### В чём разница между npm и yarn?
Это два разных менеджера npm-пакетов. Можно почитать об их отличиях [здесь](https://ua-blog.com/npm-vs-yarn-%D0%BA%D0%B0%D0%BA%D0%BE%D0%B9-%D0%BC%D0%B5%D0%BD%D0%B5%D0%B4%D0%B6%D0%B5%D1%80-%D0%BF%D0%B0%D0%BA%D0%B5%D1%82%D0%BE%D0%B2-%D1%81%D1%82%D0%BE%D0%B8%D1%82-%D0%B8%D1%81%D0%BF%D0%BE%D0%BB/) и [здесь](https://blog.risingstack.com/yarn-vs-npm-node-js-package-managers/).

<br>

#### Что лучше: npm или yarn?
На этот, как и на многие другие вопросы типа «а что лучше...?», увы, однозначного ответа нет.
> У каждого пакета есть свои достоинства и недостатки. Мы используем [yarn](https://yarnpkg.com/en/docs), так как по нашему мнению он обладает более удобным и красивым интерфейсом.

<br>

---

<br>

## ✏️ Качество кода: настройка редакторов и IDE

#### Почему редактор подсвечивает мой код?
Есть несколько возможных причин.
> `Первая`: ваш редактор расценивает код как неправильный. Это может произойти, когда вы пишете разметку JSX React без поддержки вашим редактором такого синтаксиса. Чтобы включить поддержку, нужно скачать соответствующий плагин для редактора. [Вот пример](https://atom.io/packages/language-babel) такого плагина для редактора Atom.

> `Вторая`: ваш код подсвечивает линтер, указывая на стилистические ошибки.

<br>

#### Что такое линтер?
Линтер — это статический анализатор кода.
> Он сообщает разработчику о стилистических и функциональных ошибках в программном коде. Мы используем [ESLint для JavaScript](https://eslint.org/), и [stylelint для CSS](https://stylelint.io/) . Детально о том, как работает линтер на примере ESLint можно [узнать здесь](https://www.youtube.com/watch?v=hppJw2REb8g).

<br>

<br>

#### Что такое `Prettier`? 
[`Prettier`](https://prettier.io/) — это инструмент для форматирования JavaScript-кода. Он очень быстрый и с ним легко разобраться. Больше ненужно выравнивать код вручную. Достаточно нажать сочетанию клавиш и prettier выровняет всё за тебя!

<br>

#### Как сделать, чтобы `Prettier` и `ESLint` работали вместе?
Всё не так просто.
+ У `ESLint` есть настройки, по которым он проводит анализ кода и говорит вам об ошибках.
+ Пакет [`prettier-eslint-cli`](https://github.com/prettier/prettier-eslint-cli) — это интеграция `Prettier` и `ESLint`, как мостик между двумя берегами.

```
Prettier 🏖 ← мостик prettier-eslint-cli → 🏖 ESLint
```

+ То есть, чтобы `Prettier` форматировал код по правилам `ESLint` — нужно обязательно [использовать интеграцию `prettier-eslint-cli`](https://github.com/prettier/prettier-eslint-cli#installation).

<br>
