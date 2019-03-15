# Django commands

## Create Django app

```sh
python manage.py startapp <nameapp>
```

## Show migrations

```sh
python manage.py showmigrations
```

## Create migrations

```sh
python manage.py makemigrations
```

## Run migrations

```sh
python manage.py migrate
```

## Create superuser for Django admin

```sh
python manage.py createsuperuser
```

## Create superuser for Django admin more simple

```sh
python manage.py createsuperuser --username <admin_test> --email <admin_test@mail.com>
```

## Run tests

```sh
python manage.py test
```

## Run tests with failfast

```sh
python manage.py test --failfast
```

## Go to the Shell

```sh
python manage.py shell
```

## Go to the Shell plus of [django-extensions package](https://github.com/django-extensions/django-extensions)

```sh
python manage.py shell_plus
```