FROM alpine:edge

RUN apk update && apk add --no-cache build-base=0.5-r3 zlib-dev=1.3.1-r0 gsl-dev=2.7.1-r1 bash=5.2.26-r0 perl=5.38.2-r0 autoconf=2.72-r0 automake=1.16.5-r2 make=4.4.1-r2 gcc=13.2.1_git20231014-r0 musl-dev=1.2.4_git20230717-r5 bzip2-dev=1.0.8-r6 xz-dev=5.4.6-r0 curl-dev=8.5.0-r1 openssl-dev=3.1.4-r5

RUN wget https://github.com/vcftools/vcftools/releases/download/v0.1.16/vcftools-0.1.16.tar.gz && tar -xvf vcftools-0.1.16.tar.gz && cd vcftools-0.1.16/ && ./configure && make && make install && cd .. && rm -r vcftools-0.1.16*

RUN wget https://github.com/samtools/htslib/releases/download/1.19.1/htslib-1.19.1.tar.bz2 && tar -xf htslib-1.19.1.tar.bz2 && cd htslib-1.19.1/ && make && cp bgzip /usr/local/bin/ && cd .. && rm -r htslib*

