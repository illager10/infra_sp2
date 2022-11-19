# API YaMDB

##### Проект YaMDb собирает отзывы пользователей на произведения.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
$ git clone https://github.com/illager10/infra_sp2.git
$ cd infra_sp2/infra
```
Зпалонить env-файл согласно шаблону:
```
SECRET_KEY=...
DB_ENGINE=...
DB_NAME=...
POSTGRES_USER=...
POSTGRES_PASSWORD=...
DB_HOST=...
DB_PORT=...
```

Запустить docker-compose:

```
$ docker-compose up 
```

Выполнить миграции:

```
$ docker-compose exec web python manage.py migrate
```

Заполнить бвзу данных:

```
$ docker-compose exec web python manage.py fill_tables
```

#### Технологии
  
* [Python](https://www.python.org)

* [Django REST framework](https://www.django-rest-framework.org)
