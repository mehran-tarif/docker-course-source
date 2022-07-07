# توالی اجرای کانتینرها (حل مشکل اجرای app قبل mariadb)

## توضیحات این قسمت

در این قسمت یاد میگیریم چطور مشکل وابستگی و توالی اجرای کانتینرها رو حل کنیم.

### لینک‌ها

[لینک آموزش این قسمت در یوتیوب](https://www.youtube.com/watch?v=b6R_eBNzemI)

### کامندهای استفاده شده در این قسمت

```sh
docker-compose down
```

```sh
docker-compose up --build
```

```sh
docker-compose down
```

```sh
sudo rm -rf volumes/dbdata
```

```sh
mkdir volumes/dbdata
```

```sh
docker-compose up --build
```

```sh
docker-compose down
```

```sh
docker-compose up
```