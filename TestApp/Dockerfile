FROM ubuntu:18.04

COPY . /app

WORKDIR /app


RUN apt-get update -y && \
    apt-get install --no-install-recommends -y python3.8 python-pip python3-pip python3.8-dev

RUN pip install -r requirements.txt

EXPOSE 5000

CMD FLASK_APP=./index.py FLASK_DEBUG=1 flask run --host="0.0.0.0" --port=5000