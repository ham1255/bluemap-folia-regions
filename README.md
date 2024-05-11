# paper-plugin-template

## Компиляция плагина

```shell
./gradlew build
```

Файл плагина будет находиться в `build/libs/`.
По умолчанию он называется `paper-plugin-template-<version>.jar`.

## Запуск сервера для тестирования

```shell
./gradlew runMojangMappedServer
```

Эта команда запустит сервер с Mojang маппингами без обфускации. Удобно для использования вместе с дебаггером.

Если необходимо запустить сервер с обфускацией (то, как будет выглядеть на финальном релизе, на продакшн сервере), то
можно использовать команду:

```shell
./gradlew runServer
```

## Конфигурация проекта в `gradle.properties`

* `paper.version` - версия Paper, которая будет использоваться для компиляции плагина. По
  умолчанию: `1.20.1-R0.1-SNAPSHOT`
* `paper.api` - версия Paper API, которая будет использоваться для компиляции плагина. По умолчанию: `1.20`
* `plugin.name` - название плагина, которое будет отображаться в логах и при команде `/plugins`. По
  умолчанию: `example-plugin`
* `plugin.group` - группа плагина. По умолчанию: `io.pfaumc.example`
* `plugin.version` - версия плагина. По умолчанию: `1.0-SNAPSHOT`
* `plugin.main` - основной класс плагина. По умолчанию: `io.pfaumc.example.ExamplePlugin`
