FROM ubuntu:focal


RUN apt-get update 

RUN curl -sL https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh -o install_nvm.sh

RUN bash install_nvm.sh && source ~/.profile

RUN nvm install --lts
