FROM python:alpine3.8

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 5000

CMD FLASK_APP=./index.py FLASK_DEBUG=1 flask run --host="0.0.0.0" --port=5000 