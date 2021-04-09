Z8 Tutorial - обучающий проект на базе фреймворка [Z8](https://github.com/zenframework/z8/), содержащий исходные коды к курсу вебинаров, опубликованных на канале [Z8 Zenframework](https://www.youtube.com/channel/UCEpz5os7yrpCQ6G0Gqek_QQ). Каждому вебинару соответствует отдельная ветка Git.

Описание фреймворка Z8, а также импорт проекта Z8 Tutorial приведено в [Wiki проекта Z8](https://github.com/zenframework/z8/wiki).

# Как собрать и запустить проект Z8 Tutorial

Склонируйте [Z8](https://github.com/zenframework/z8/) на свой диск.

Скопируйте _gradle.properties.default_ в _gradle.properties_ и выберите один из вариантов сборки:
1. С использованием исходных кодов Z8 из Git-репозитория - свойство _z8.home_ должно содержать полный путь к каталогу исходных кодов Z8, склонированных по выше приведённой ссылке.
2. С использованием бинарных библиотек Z8 - свойство _z8.home_ НЕ должно быть установлено.

Запустите команду сборки и запуска: gradlew run

Откройте веб-браузер (предпочтителен Google Chrome) и перейдите по ссылке http://localhost:9080

## Конфигурация Eclipse Workspace
1. Если вы используете исходные коды Z8, проект должен находиться в Eclipse Workspace.
2. Если вы используете бинарные библиотеки Z8, в Eclipse Workspace должен находиться только проект _org.zenframework.z8.lang_. Остальные зависимости будут автоматически загружены сборщиком Gradle из Maven-репозитория через Интернет.

# Z8 Tutorial Project Build How-to

Clone [Z8](https://github.com/zenframework/z8/) to your disk.

Copy _gradle.properties.default_ to _gradle.properties_ then choose one of project building options.

You have 2 options to develop Z8 project:
1. Using Z8 Project sources from Git - _z8.home_ must point to Z8 Project folder, cloned from link above.
2. Using Z8 Project binaries - _z8Home_ must not be set.

Build & run project: gradlew run

Open browser (Google Chrome preferred) and go to http://localhost:9080

## Eclipse workspace configuration:
1. If you use Z8 Project sources, Z8 Project must be in the same workspace.
2. If you use Z8 Project binaries, subproject _org.zenframework.z8.lang_ must be in the same workspace. Other Z8 dependencies are resolved with Gradle Maven plugin.
