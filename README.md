# Docker_homework

1. Скачать образ posgres (docker pull postgres)
2. Переменное окружение (docker run --name db_django -p 5432:5432 -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=public -e
   POSTGRES_HOST_AUTH_METOHOD=md5 postgres)
3. Скачать образ python с подключением сети контейнера к сети локальной машины (docker run --network host -it python bash)
4. Установка django (pip install django)
5. Установка библиотеки для работы с postgres(pip install psycopg2)
6. Создание проекта (django-admin startproject Docker)
7. Переходим в директорию приложения (cd Docker)
8. Установка редактора nano для подключения БД в settings.py(apt-get update, apt-get install nano)
9. Редактирование DATABASE в settings.py с помощью nano (nano Docker/settings.py)
10. Запуска миграции в базе данных (./manage.py migrate)
11. Запуск сервера (./manage.py runserver)