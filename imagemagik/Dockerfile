FROM alpine:edge

RUN apk update && apk add --no-cache build-base=0.5-r3 bash=5.2.26-r0 

RUN apk add --no-cache --virtual .build-deps imagemagick-dev

RUN apk add imagemagick

RUN apk add ghostscript=10.02.1-r0 

