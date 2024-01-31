# Kittygram
## Описание
<a href='https://kittydocker.ddns.net'>Kittygram </a> предоставляет пользователям возможность публиковать изображения своих любимых котиков! 

## Технологии:
HTML, CSS, JavaScript, Python, Django, React, Docker.

## Запуcк
Для запуска проекта воспользуемся Linux(Ubuntu)
### Клонирование
Клонируйте репозиторий
```
git clone git@github.com:ponyk1ller/kittygram_final.git
```
### Подготовка виртуального окружения
Создаем окружения для проекта
```
sudo nano .env
```
```
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_NAME=kittygram

DB_HOST=db
DB_PORT=5432

SECRET_KEY='django-insecure-cg6*%6d51ef8f#4!r3*$vmxm4)abgjw8mo!4y-q*uq1!4$-89$'
DEBUG = 'True'
ALLOWED_HOSTS = '127.0.0.1'
```
### Запуск Docker compose 
В директории проекта запускаем docker-compose.production.yml
```
sudo docker compose up -f docker-compose.production.yml up
```
## Конфигурационные файлы
Во время разработки рекомендуется использовать <strong>docker-compose.yml</strong>, где образы билдятся при каждом запуске.
В продакшене использовать <strong>docker-compose.production.yml</strong> для получения готовых образов с Docker Hub.



## Автор
Халиуллин Ильяс