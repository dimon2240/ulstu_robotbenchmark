# ulstu_robotbenchmark

Развернуть и запустить проект
~~~
cd docker
cp .env.example .env
docker compose build
docker compose up -d
~~~
После запуска перейти на 127.0.0.1:8047

Сейчас доступны контейнеры с webots, php и nginx. Дефолтный порт сервера 8047

TODO list
- ~~Загрузить мир из открытого github репозитория~~
- ~~Загрузить локальный мир~~
- ~~Разобраться с редактором контроллера~~
- ~~Подключить инструкцию и метрики к упражнению~~
- Разобраться с Supervisor API
- Создать свое тестовое упражнение