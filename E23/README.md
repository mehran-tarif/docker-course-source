# داکرایز کردن nodejs و دیتابیس mongo (آماده سازی پروژه)

## توضیحات این قسمت

در این قسمت داکرایز پروژه nodejs رو شروع می کنیم: ابتدا پروژه مربوطه رو دانلود و mongodb رو روی سرویس داکر بالا میاریم، در قدم بعدی، که میشه جلسه بعد، یه پک داکرش می کنیم.


### لینک‌ها

[لینک آموزش این قسمت در یوتیوب](https://www.youtube.com/watch?v=KID0hoAW7_E)

[لینک پروژه موردنظر در گیت هاب](https://github.com/jatinbharadwaj/blog-app)

[لینک دریافت پکیج Nodejs](https://nodejs.org/en/download/)

[لینک پلی لیست آموزش دیتابیس mongo سیلیسیوم](https://www.youtube.com/playlist?list=PLAt10Vana3Yfq0eUrJn7wZEdMG49MyB_j)

[لینک داکر mongo](https://hub.docker.com/_/mongo)

### کامندهای استفاده شده در این قسمت

```sh
sudo apt install nodejs npm
```

```sh
npm install
```

```sh
npm start
```

```sh
docker run -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=pass --name mongodb -d mongo
```