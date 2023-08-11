FROM debian:bullseye
RUN  export DEBIAN_FRONTEND=noninteractive

RUN apt-get -y update
RUN apt-get -y upgrade

RUN apt-get -y install build-essential tmux gcc fish
RUN apt clean 
ENV TERM xterm
EXPOSE  22
