FROM python:3.10-alpine

RUN apk update && apk add --no-cache python3 py3-pip bash poppler poppler-utils g++ pkgconfig cmake poppler-dev && pip install --no-cache-dir --upgrade pip 

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt
