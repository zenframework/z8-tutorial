Z8 Tutorial - проекта на базе фреймворка [Z8](https://github.com/zenframework/z8/), содержащий исходные коды к курсу вебинаров, опубликованных на канале [Z8 Zenframework](https://www.youtube.com/channel/UCEpz5os7yrpCQ6G0Gqek_QQ)

Каждому вебинару соответствует отдельная ветка Git.

Описание фреймворка Z8, а также проекта Z8 Template приведено в [Wiki проекта Z8](https://github.com/zenframework/z8/wiki)

# Z8 Tutorial Project Build How-to

Copy _gradle.properties.default_ to _gradle.properties_ then choose one of project building options.

You have 2 options to develope Z8 porject:
1. Using Z8 Project sources from Git - _z8.home_ must point to Z8 Project folder, Gradle build script assumes Z8 Project is in Eclipse workspace
1. Using Z8 Project binaries - _z8Home_ must not be set

Eclipse workspace configuration:
1. If you use Z8 Project sources, Z8 Project must be in the same workspace.
1. If you use Z8 Project binaries, subproject _org.zenframework.z8.lang_ must be in the same workspace. Other Z8 dependencies are resolved with Gradle Maven plugin.
