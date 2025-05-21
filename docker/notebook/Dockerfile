# FROM debian:10
FROM jupyter/pyspark-notebook:latest

WORKDIR /notebook

COPY ./docker/notebook/requirements.txt /tmp/requirements.txt
COPY .env /.env

RUN pip3 install -r /tmp/requirements.txt
