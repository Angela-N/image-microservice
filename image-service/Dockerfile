FROM python:3.8

WORKDIR /app

COPY ./requirements.txt /app/requirements.txt

RUN apt-get update \
    && apt-get install gcc -y \
    && apt-get clean

RUN apt-get update && apt-get install tk-dev && rm -r /var/lib/apt/lists/*

RUN pip install -r /app/requirements.txt \
RUN pip3 install -r /app/requirements.txt \
    && rm -rf /root/.cache/pip



ENV PYTHONPATH "${PYTHONPATH}:/code"

COPY . /app/