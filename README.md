## Инструкция

После всего того что я проделал(Скопировал проект,добавил настройки в опен сервер,PHPmyadmin добавил базу данных и тд.)

### В корне проекта создаю файл .env и изменяю следующие настройки: 

#### APP_URL=http://mysmartprofit.com.local
#### DB_DATABASE=mysmartprofit
#### DB_USERNAME=root
#### DB_PASSWORD=root

#### CACHE_DRIVER=file

#### SESSION_DRIVER=file

### Устанавливаю 
```shell
 composer install
```
### Понижаю до версии 1 
```shell
composer self-update --1
```
### При появлении проблем можно еще поигратся 
```shell
composer update
```
### Проверяю версию, если 1 с хвостиком огонь
```shell
composer -v
```
### Запускаю эту хренотень. И ЭТО ВСЕ В КОНСОЛЕ ОПЕН СЕРВЕРА!!!!!
```shell
php artisan key:generate && php artisan storage:link && php artisan ide-helper:generate && php artisan ide-helper:meta
```
### Потом

```shell
npm run prod
npm run watch
```
и молимся чтобы заработало 🤞🙌

