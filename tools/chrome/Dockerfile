# FROM resin/rpi-raspbian:wheezy
FROM armhf/alpine
RUN useradd -ms /bin/bash chromium

RUN apt-get update && apt-get dist-upgrade && apt-get install -y \
    chromium-browser \
    lsb-release

USER chromium