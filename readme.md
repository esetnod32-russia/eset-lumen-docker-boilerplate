# Lumen PHP Framework for Eset with   Docker container

### Работа с котейнерами если нужно развернуть проект на локали (Стек php-fpm7.1, Nginx,  Mysql5.7.*, docker), когда нет возможности работать на dev площадке.

- Склонировать репку - git@github.com:esetnod32-russia/eset-lumen.git

- Установить Docker и Docker-compose на локалные машины (Windows - https://docs.docker.com/compose/install/) для (MacOs - https://docs.docker.com/compose/install/) для (Linux - https://docs.docker.com/compose/install/)

- Перейдем в репозиторий `cd eset-lumen ` далее копируем файл конфигурации приложения `сp .env.example .env` устанавливаем зависимости `composer install`

- Далее выполним `docker-compose` если все нормально видим команды docker-compose (если машина не знает такой команды тогда проолжаем устанавливать правильно docker-compose), тогда начинаем сборку контейнера у себя на локали займет меньше минуты выполнив команду `docker-compose up -d` после сборки выполним команду `docker ps` и увидим там 3 контейнера значит все ок, вы молодец xD

- Теперь осталось накотить миграции `php artisan migrate --env=console` 

- Далее в файле переходим на http://127.0.0.1/ порт-80 







