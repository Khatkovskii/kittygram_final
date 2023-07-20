![workflow](https://github.com/Khatkovskii/kittygram_final/actions/workflows/main.yml/badge.svg)

# Kittygram
Социальная сеть для владельцов котов, кошек и не только.

## Запуск проекта в dev-режиме
Клонируйте репозиторий и перейдите в него в командной строке:
```
git clone
cd kittygram_final
```
Запустите проект с помощью команды:
```
docker compose up
```
Примените миграции с помощью команды:
```
docker compose exec backend python manage.py migrate
```
Соберите статику Django с помощью команды:
```
docker compose exec backend python manage.py collectstatic
```
Скопируйте статику командой:
```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```
Сайт будет доступен по адресу:
http://127.0.0.1:9000/

## Автор проекта
[Khatkovskii](https://github.com/Khatkovskii) 