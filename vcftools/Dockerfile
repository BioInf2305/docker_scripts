FROM alpine:edge

RUN apk update && apk add --no-cache build-base=0.5-r3 && apk add --no-cache zlib-dev=1.3.1-r0 && apk add --no-cache gsl-dev=2.7.1-r1 && apk add --no-cache bash=5.2.26-r0 && apk add --no-cache perl=5.38.2-r0

RUN wget https://github.com/vcftools/vcftools/releases/download/v0.1.16/vcftools-0.1.16.tar.gz && tar -xvf vcftools-0.1.16.tar.gz

RUN cd vcftools-0.1.16/ && ./configure && make && make install && cd .. && rm -r vcftools-0.1.16*

