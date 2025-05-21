# FROM debian:10
FROM jupyter/pyspark-notebook:latest

WORKDIR /notebook

COPY ./docker/notebook/requirements.txt /tmp/requirements.txt
COPY .env /.env

# RUN sudo -S 'r13l02c1988' apt-get update && apt-get install -y \
#     build-essential \
#     curl \
#     libpq-dev 

RUN pip3 install -r /tmp/requirements.txt
