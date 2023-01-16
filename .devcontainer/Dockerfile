FROM ubuntu:focal

RUN apt-get update \
    && apt-get -y install --no-install-recommends \
    curl \
    git-core \
    gnupg \
    locales \
    wget \
    tree \
    jq \
    fontconfig \
    # set up locale
    && locale-gen en_US.UTF-8 && fc-cache -vf
    && curl -sL https://deb.nodesource.com/setup_18.x -o /tmp/nodesource_setup.sh


RUN bash /tmp/nodesource_setup.sh

RUN apt install nodejs
