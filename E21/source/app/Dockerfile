FROM python:alpine

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
ENV DJANGO_SUPERUSER_PASSWORD admin

RUN mkdir /app
WORKDIR /app

RUN apk update
RUN apk add --no-cache gcc python3-dev musl-dev mariadb-dev

RUN pip install --upgrade pip
RUN pip install django gunicorn mysqlclient

RUN apk del gcc python3-dev musl-dev

CMD while ! python3 manage.py sqlflush > /dev/null 2>&1 ; do sleep 1; done && \
    python3 manage.py makemigrations --noinput && \
    python3 manage.py migrate --noinput && \
    python3 manage.py collectstatic --noinput && \
    python3 manage.py createsuperuser --user admin --email admin@localhost --noinput; \
    gunicorn -b 0.0.0.0:8000 config.wsgi