## создание пустого проекта
В папке с проектом выполнить команду
```shell
composer create-project laravel/laravel .
phpartisan install:api
php artisan config:publish cors
php artisan storage:link
```

В корне проекта создать файл .htaccess
```php
RewriteEngine on
RewriteRule ^(.*)$ public/$1 [L]
```
