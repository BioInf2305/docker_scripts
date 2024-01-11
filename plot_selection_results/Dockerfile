FROM python:3.10-alpine

RUN apk update && apk add python3 py3-pip

RUN pip install --no-cache-dir --upgrade pip

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt
