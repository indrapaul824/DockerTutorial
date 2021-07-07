FROM ubuntu:18.04

COPY . /app

WORKDIR /app

RUN apt-get update -y
RUN apt-get install -y python3-pip libssl-dev libffi-dev python3-dev build-essential

RUN pip3 install --upgrade pip
RUN pip3 install -r requirements.txt

EXPOSE 5000

CMD FLASK_APP=./index.py FLASK_DEBUG=1 flask run --host="0.0.0.0" --port=5000 