FROM mcr.microsoft.com/devcontainers/base:debian
RUN export DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get -y install git

# RUN mkdir /home/workdir
# RUN git clone git://git.buildroot.net/buildroot -b 2022.08.2 /home/workdir/buildroot/

RUN apt-get -y install build-essential ncurses-dev unzip git atfs tftpd-hpa
RUN apt-get -y install gperf autoconf flex texinfo help2man libtool libtool-bin bison
RUN apt-get -y install libsqlite3-dev cpio bc
# just for build docs
RUN apt-get -y install asciidoc w3m
RUN apt clean 