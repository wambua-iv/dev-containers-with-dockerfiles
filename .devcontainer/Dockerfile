FROM node:lts-hydrogen

RUN echo 'deb http://security.debian.org/debian-security bullseye-security main contrib non-free' >> /etc/apt/sources.list \
    apt-get update \
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


RUN echo 'done'
