#  داکرایز کردن nodejs و دیتابیس mongo (نوشتن داکر کامپوز)

## توضیحات این قسمت

در این جلسه به طور کامل nodejs رو همراه با mongodb داکرایز می کنیم.

این قسمت تکمیل کننده [قسمت قبلی](../E23/) است.

فایل‌های پروژه nodejs به دلیل حجم زیاد قرار نگرفته و از طریق لینک زیر می‌توانید آن را دریافت کنید.

### لینک‌ها

[لینک آموزش این قسمت در یوتیوب](https://www.youtube.com/watch?v=E4e96gDXPOU)

[لینک پروژه موردنظر در گیت هاب](https://github.com/jatinbharadwaj/blog-app)

[لینک داکر node](https://hub.docker.com/_/node)

### کامندهای استفاده شده در این قسمت

```sh
docker pull node:alpine3.12
```

```sh
touch docker-compose.yml
```

```sh
mkdir app
```

```sh
mkdir -p volumes/db
```

```sh
cd app
```

```sh
touch Dockerfile
```

```sh
docker-compose up --build
```