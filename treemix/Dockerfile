FROM alpine:edge

RUN apk update && apk add build-base=0.5-r3 && apk add zlib-dev=1.3-r2 && apk add gsl-dev=2.7.1-r1 && apk add boost-dev=1.82.0-r3

RUN wget https://bitbucket.org/nygcresearch/treemix/downloads/treemix-1.13.tar.gz && tar -xvf treemix-1.13.tar.gz

RUN cd treemix-1.13 && ./configure && make && cp ./src/treemix /usr/local/bin/ && cd .. && rm -r treemix-1.1*

