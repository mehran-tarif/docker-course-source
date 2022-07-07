# تنظیمات مهم پروژه جنگو برای داکرایز کردنش

## توضیحات این قسمت

در این جلسه با تنظیمات مهم جنگو قبل داکرایز کردنش آشنا میشیم.

### لینک‌ها

[لینک آموزش این قسمت در یوتیوب](https://www.youtube.com/watch?v=StCX8qMPBJo)

[مستندات فایل‌های استاتیک جنگو](https://docs.djangoproject.com/en/3.2/howto/static-files/)

### کامندهای استفاده شده در این قسمت

```sh
virtualenv -p python3 .venv
```

```sh
source ~/.venv/bin/activate
```

```sh
pip install django gunicorn
```

```sh
django-admin startproject config
```

```sh
mv config app
```

```sh
cd app
```

```sh
./manage.py runserver
```

```sh
gunicorn -b 0.0.0.0:8000 config.wsgi
```

```sh
./manage.py collectstatic
```

```sh
gunicorn -b 0.0.0.0:8000 config.wsgi
```

```sh
./manage.py makemigrations
```

```sh
./manage.py migrate
```

```sh
./manage.py collectstatic
```

```sh
./manage.py collectstatic --noinput
```

```sh
./manage.py createsuperuser --noinput
```

```sh
./manage.py createsuperuser --noinput --user admin
```

```sh
./manage.py createsuperuser --noinput --user admin --email admin@localhost
```

```sh
rm db.sqlite3
```

```sh
export DJANGO_SUPERUSER_PASSWORD=admin
```

```sh
./manage.py migrate --noinput
```

```sh
./manage.py createsuperuser --noinput --user admin --email admin@localhost
```