Установка базовых пакетов и плагинов

Плагин для точного автодополнения

https://github.com/barryvdh/laravel-ide-helper
```
composer require --dev barryvdh/laravel-ide-helper
```

Добавить в Composer.json в раздел Scripts
```
"post-update-cmd": [
    "Illuminate\\Foundation\\ComposerScripts::postUpdate",
    "@php artisan ide-helper:generate",
    "@php artisan ide-helper:meta"
]
```

Обновление изменений в Composer.json
```
composer update
```

Отображение DebugBar на странице в режиме Dev

https://github.com/barryvdh/laravel-debugbar

```
composer require barryvdh/laravel-debugbar --dev
```

Запись данных по подключению к БД в файле .env
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=poligon
DB_USERNAME=root
DB_PASSWORD=
```
