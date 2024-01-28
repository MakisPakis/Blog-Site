Как развернуть проект используя Docker
Клонировать репозиторий
Прописать свои ключи и данные в файле .env.dev
Cоздание образа с контейнерами
docker compose -f docker-compose.dev.yml build
Запуск контейнеров
docker compose -f docker-compose.dev.yml up
После запуска в доп терминале можно прописать 
docker exec -it django sh для запуска терминала
И создать суперюзера для доступка к админке
python manage.py createsuperuser
