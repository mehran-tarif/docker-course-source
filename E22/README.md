# داکرایز کردن وردپرس با lamp (php و apache و mysql)

## توضیحات این قسمت

در این قسمت کانفیگ LAMP (لینوکس، آپاچی، mysql و php) رو داریم و میخواییم محبوب ترین CMS دنیا رو باهاش لود کنیم. طبیعتا شما که تا اینجا اومدید، میتونید با دستکاری پوشه مربوط به فایل های wp سایر اسکریپت های php تون رو هم لود کنید.


### لینک‌ها

[لینک آموزش این قسمت در یوتیوب](https://www.youtube.com/watch?v=pdXgsD9ALTs)

[لینک داکر وردپرس](https://hub.docker.com/_/wordpress)

### کامندهای استفاده شده در این قسمت

```sh
touch docker-compose.yml
```

```sh
mkdir -p ./volumes/wordpress ./volumes/dbdata
```

```sh
docker-compose up --build
```