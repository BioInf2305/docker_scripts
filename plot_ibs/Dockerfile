FROM python:3.10-alpine

RUN apk update && apk add python3 py3-pip gcc=13.2.1_git20231014-r0 libc-dev=0.7.2-r5 bash

RUN pip install --no-cache-dir --upgrade pip

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt
