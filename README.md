# ulstu_robotbenchmark

Развернуть и запустить проект
~~~
cd docker
cp .env.example .env
docker compose build
docker compose up -d
~~~
После запуска перейти на 127.0.0.1:8047

Папка с проектами монтируется внутрь контейнера webots

Сейчас доступны контейнеры с webots, php и nginx. Дефолтный порт сервера 8047

TODO list
- ~~Упаковать webots в докер~~
- ~~Загрузить симуляцию из открытого github репозитория~~
- ~~Загрузить локальную симуляцию~~
- ~~Разобраться с редактором контроллера~~
- ~~Разобраться с Supervisor API~~
- ~~Создать свое тестовое упражнение~~
- ~~Подключить инструкцию и метрики к своему упражнению~~
- Написать свой бек (думаю будет проще, чем отлаживать robotbenchmark)
  - Авторизация/регистрация
  - Список доступных упражнений
  - Сохранение результатов упражнений
  - АПИ для получения результатов упражнений, интеграция с дневником КШ ФИСТ

Известные проблемы
  - Почему-то иногда webots зависает и висит бесконечное "Starting simulation". 
    Чтобы пофиксить надо убрать монтирование всех томов в webots, перезапустить контейнер, потом вернуть обратно. 
    С чем это связано пока не разобрался.
    