FROM rocker/r-ubuntu:jammy

RUN apt-get update

COPY ./install_packages.r /home/

RUN Rscript /home/install_packages.r
