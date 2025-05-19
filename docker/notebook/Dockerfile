# FROM debian:10
FROM python:3.11-slim

WORKDIR /notebook

COPY ./docker/notebook/requirements.txt /tmp/requirements.txt
COPY ./.env /.env

# RUN apk add --no-cache git
RUN pip3 install --no-cache-dir -r /tmp/requirements.txt

# ENV PYTHONUNBUFFERED=1
# RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
# RUN python3 -m ensurepip
# RUN pip3 install --no-cache --upgrade pip setuptools

# RUN apt update && apt install -y \
#      build-essential \
#      curl \
#      libpq-dev \
#      python3 \
#      python3-pip \
#      && rm -rf /var/lib/apt/lists/* 

# RUN pip3 install -r /tmp/requirements.txt

# CMD ["jupyter", "lab"]