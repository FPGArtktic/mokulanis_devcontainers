FROM debian:bullseye
RUN  export DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update
RUN apt-get -y upgrade

RUN apt-get -y install build-essential tmux gcc fish \
    autoconf \    
    cmake \
    git \
    g++ \
    libstdc++6 \
    libboost-dev \
    libdb-dev \
    libffi-dev \
    libfreetype6-dev \
    libjpeg-dev \
    libpng-dev \
    libprotobuf-dev \
    libssl-dev \
    libsqlite3-dev \
    clang \
    clang-format 
    
RUN apt clean 
ENV TERM xterm
EXPOSE  22
