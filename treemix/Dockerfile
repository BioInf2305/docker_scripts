FROM alpine:edge

RUN apk update && apk add --no-cache build-base=0.5-r3 && apk add --no-cache zlib-dev=1.3.1-r0 && apk add --no-cache gsl-dev=2.7.1-r1 && apk add --no-cache boost-dev=1.82.0-r3 && apk add --no-cache bash=5.2.26-r0

RUN wget https://bitbucket.org/nygcresearch/treemix/downloads/treemix-1.13.tar.gz && tar -xvf treemix-1.13.tar.gz

RUN cd treemix-1.13 && ./configure && make && cp ./src/treemix /usr/local/bin/ && cd .. && rm -r treemix-1.1*

