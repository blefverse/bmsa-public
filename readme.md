# Blefonix RP Public

[![sampctl](https://img.shields.io/badge/sampctl-brpsa--public-2f2f2f.svg?style=for-the-badge)](https://github.com/brpsamp/brpsa-public)

*The Russian version is below.*
*Версия на русском ниже.*

**The official Blefonix RolePlay public repository. Updates are welcome. If bugs, create an issue.**

## Vision of the project

We see Blefonix RP as something fresh, unusual behind its meaning and game design. We do not set ourselves the goal of making another copy of some popular mod. We want to make our own, popular in the future mod. We, as founders, do not have a lot of money for development, but we have big ideas and a desire to create the RP project of our dreams. We are driven by the idea of helping players with their personal development. Playing, one will not only have fun, but also a useful experience that can be used in the real world.

A little later on this page will be a description of the capabilities of the mod itself, which systems are present, and other things. Welcome!

Feel free to edit this file, as well as the mod itself, if you have any interesting ideas.

## About the source code

Please keep code as clean as possible, stick to our style:
- Use "{" next to the function name.
- Sometimes you can use code next to "}".
- Separate values with a space.
- If a function has only one subfunc - you should write them in one line.
- "LANG_STRING" instead of "text".
- Text itself should be added to scriptfiles/*.ini – other people will take care of translation into other langs.
- Use possibilities pawn.cmd/zlang/mdialog/skinselector/other instead of classic ones.

If you have an idea what to add or change, but you are not able to implement it yourself - write to this [chat in discord]().

## What technologies do we use

* Main lang Pawn
* IDE: vscode
* Platforms: open.mp samp ugmp
* [sampctl](https://github.com/Southclaws/sampctl)
* zlang+mdialog+gvar
* streamer
* Pawn.CMD
* YSF+SKY

## Installation

### Requirements

To start working with this mod, the following tools must be installed on your computer:

- [sampctl](https://github.com/Southclaws/sampctl) For automatic installation of necessary Pawn dependencies and SA-MP plugins.
- [vscode](https://code.visualstudio.com/) For convenient code editing. After installing it, we also recommend installing [sampctl plugin](https://marketplace.visualstudio.com/items?itemName=southclaws.vscode-pawn). You can use any other editor you like.
- [xampp](https://apachefriends.org/) To import a database and connect to it. You can use any other analogue, for example [OpenServer](https://ospanel.io/).

### Build mod for the first time

Clone the repository to your computer using [GitHub Desktop](https://desktop.github.com/).

Now open the mod folder in your favorite code writing environment. We recommend [vscode](https://code.visualstudio.com/). It has a built-in command line (terminal) with which you can do various quick actions thanks to sampctl, for example you can compile (`ctrl+shift+b`) and also start the server. The normal Pawno editor is not to be used, but [you can use this one](https://github.com/pawn-lang/compiler/releases/tag/v3.10.10).

Now be sure to enter the phpMyAdmin panel through, for example, xampp. Immediately after logging in at the top, click on `Databases` and specify the name `brpsa_invite`, compare/encode `utf8mb4_general_ci`, and click Create. Done!

Now run the following commands at the command line to get the project's dependencies, as well as update plugins, to get the current compiler version, and run other necessary components. If you use vscode, you can open the terminal with ``shift+ctrl+~`.

```
sampctl p ensure
sampctl p build
```

If you do not see all files and folders in vscode, it's okay. You have installed the recommended extension [Explorer Exclude](https://marketplace.visualstudio.com/items?itemName=RedVanWorkshop.explorer-exclude-vscode-extension).

## Server Running

If you have compiled the mod without errors, you can start the server with samp-server.exe, but we recommend that you start the server with the following command.

```
sampctl p run
```

Speaking of ``server.cfg''. Do not edit it! This is now a generated file. You should now use the `pawn.json` file to edit the server configuration. Read more about pawn.json on the official [sampctl](https://github.com/Southclaws/sampctl) pages.

---

---

## Russian Description

**Официальный публичный репозиторий Blefonix RolePlay. Обновления приветствуются. Если нашли баг, создайте issue.**

## Видение проекта

Мы видим Blefonix RP как что-то свежее, необычное за своим смыслом и гейм-дизайном. Мы не ставим перед собою цель сделать очередную копию какого-либо популярного мода. Мы хотим сделать свой, популярный в будущем мод. У нас, как основателей, нет больших средств на разработку, но есть большие идеи и желание создать RP проект мечты. Нами движет идея помощи игрокам с их личностным развитием. Играя, человек будет получать не только удовольствие, но и полезный опыт, который сможет использовать в реальном мире. Именно поэтому был создан публичный репозиторий, чтобы проект также развивало и компьюнити.

Чуть позже на данной странице появится описание возможностей самого мода, какие системы тут присутствуют, и всякое другое. Добро пожаловать!

## Об исходном коде

Просим по возможности соблюдать чистоту в коде и придерживаться нашей стилистики:
- Пишите "{" сразу возле названия функции.
- Иногда возможно использование кода сразу после "}".
- После значение, т.е. запятые и подобное разделяйте пробелом.
- Если внутри функции только одна подфункция – стоит писать их в одну строку.
- Вместо текста нужно писать языковые переменные (сам текст добавляйте в scriptfiles/lang_*.ini – переводом на другие языки позаботятся другие люди).
- Используйте возможности pawn.cmd/zlang/mdialog/skinselector/прочего вместо классических.

```
Файлы перевода на русский используют кодировку windows1251. Откройте их в своём редакторе для просмотра содержимого без иероглифов.
```
```
Если желаете сравнить версии файлов, используйте для этого также редактор, иначе неправильно отобразится кириллица.
```

Если у вас есть идеи, что добавить либо изменить, но вы не в состоянии это самостоятельно реализовать — напишите в данный [чат в дискорде]().

Смело редактируйте данный файл, также как и сам мод, если у вас появились какие-либо интересные идеи.

## Какие технологии используем

* ЯП — Pawn
* IDE — VS Code
* Платформы — open.mp / samp / ugmp
* [sampctl](https://github.com/Southclaws/sampctl)
* zlang+mdialog+gvar
* streamer
* Pawn.CMD
* YSF+SKY

## Установка

### Требования

Чтобы начать работу с данным модом, на вашем компьютере должны быть установлены следующие инструменты:

- [sampctl](https://github.com/Southclaws/sampctl) Для автоматической установки необходимых зависимостей Pawn и плагинов SA-MP.
- [vscode](https://code.visualstudio.com/) Для удобного редактирования кода. После его установки, рекомендуем также установить [плагин sampctl](https://marketplace.visualstudio.com/items?itemName=southclaws.vscode-pawn). Вы можете использовать любой другой удобный вам редактор.
- [xampp](https://apachefriends.org/) Для импорта базы данных и подключения к ней. Вы можете использовать любой другой аналог, например, [OpenServer](https://ospanel.io/).

### Сборка мода в первый раз

Клонируйте репозиторий на свой компьютер с помощью [GitHub Desktop](https://desktop.github.com/).

Теперь откройте папку с модом в своей любимой среде написания кода. Рекомендуем [vscode](https://code.visualstudio.com/). У него есть встроенная командная строка (терминал), с помощью которого благодаря sampctl можно выполнять различные быстрые действия, например, можно выполнять компиляцию (`ctrl+shift+b`), а также запускать сервер. Обычный редактор Pawno использовать не жально, но [можно этот](https://github.com/pawn-lang/compiler/releases/tag/v3.10.10).

Теперь обязательно войдите в панель phpMyAdmin через, например, xampp. Сразу после входа вверху кликните на `Базы данных` и укажите название `brpsa_invite`, сравнение/кодировку `utf8mb4_general_ci`, и кликните Создать. Готово!

Теперь выполните следующие команды в командной строке для получения зависимостей проекта, а также обновления плагинов, для получения актуальной версии компилятора, и выполнения других необходимых компонентов. Если используете vscode, то терминал можно открыть с помощью `shift+ctrl+~`.

```
sampctl p ensure
sampctl p build
```

Если у вас не отображаются все файлы и папки в vscode — это нормально. Вы установили рекомендуемое расширение [Explorer Exclude](https://marketplace.visualstudio.com/items?itemName=RedVanWorkshop.explorer-exclude-vscode-extension).

## Запуск сервера

Если компиляция мода была выполнена без ошибок, вы можете запустить сервер с помощью samp-server.exe, но мы рекомендуем запускать сервер с помощью следующей команды:

```
sampctl p run
```

Кстати о `server.cfg`. Не редактируйте его! Теперь это генерируемый файл. Теперь вы должны использовать файл `pawn.json` для редактирования конфигурации сервера. Более подробно о pawn.json читайте на официальных страницах [sampctl](https://github.com/Southclaws/sampctl).
