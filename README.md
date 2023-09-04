# hmwrk-parsing
Парсер результатов домашних заданий с api Онлайн-школы
Перед запуском скрипта нужно установить библиотеки:

    pip install datetime aiohttp asyncio bs4 configparser csv re lxml
Также необходимо настроить config.ini по шаблону:

    [main]
    email = ***@100points.ru # почта (логин)
    password = *** # пароль
    course_id = ** # id курса
    [email]
    filling_in_the_template = true
    count = 2 # кол-во учеников
    item1 = ...
    item2 = ...
    # кол-во item должно соответствовать кол-ву учеников
Программа потребует на ввод номер модуля и урока

Результат работы скрипта сохраняет в формате {номер модуля}-{номер урока}--{дата}.csv
