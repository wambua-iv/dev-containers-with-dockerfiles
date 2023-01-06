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

RUN wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

RUN bash install_nvm.sh && source ~/.profile

RUN nvm install --lts
