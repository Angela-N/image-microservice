FROM python:3.8-slim

WORKDIR /app

COPY ./requirements.txt /app/requirements.txt

RUN apt-get update \
    && apt-get install gcc -y \
    && apt-get clean \
    && apt-get install tk

RUN pip install -r /app/requirements.txt \
    && rm -rf /root/.cache/pip

RUN pip3 install Pillow


COPY . /app/