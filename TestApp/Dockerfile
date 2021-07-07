FROM ubuntu:18.04

COPY . /app

WORKDIR /app

RUN apt-get update && \
    apt-get install python3 python3-pip python3-dev -y

ENV export LC_ALL=C.UTF-8 
ENV export LANG=C.UTF-8

RUN pip3 install --upgrade pip
RUN pip3 install -r requirements.txt

EXPOSE 5000

CMD FLASK_APP=./index.py FLASK_DEBUG=1 flask run --host="0.0.0.0" --port=5000 