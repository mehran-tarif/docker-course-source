FROM python:alpine

RUN mkdir /app
ADD ./app.py /app 

WORKDIR /app

RUN pip install --upgrade pip
RUN pip install flask gunicorn

CMD gunicorn -b 0.0.0.0:5000 app:app