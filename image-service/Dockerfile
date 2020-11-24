FROM python:3.8-slim

WORKDIR /app

COPY ./requirements.txt /app/requirements.txt

RUN apt-get update \
    && apt-get install gcc -y \
    && apt-get clean

RUN pip3 install -r /app/requirements.txt \
    && rm -rf /root/.cache/pip

COPY . /app/