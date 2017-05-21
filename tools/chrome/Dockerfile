FROM resin/rpi-raspbian:wheezy
RUN useradd -ms /bin/bash chromium
RUN apt-get update && apt-get dist-upgrade && apt-get install -y \
    rpi-update \
    chromium-browser \
    lsb-release && rm -rf /var/lib/apt/lists/*

RUN rpi-update

USER chromium

FROM resin/rpi-raspbian:jessie
RUN useradd -ms /bin/bash chromium
RUN sudo apt-get update && apt-get install -y \
    wget \
    rpi-update \
    ttf-mscorefonts-installer \
    chromium-browser \
    lsb-release

RUN rpi-update

USER chromium