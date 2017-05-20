FROM resin/rpi-raspbian:jessie
RUN useradd -ms /bin/bash chromium
RUN apt-get update && apt-get dist-upgrade && apt-get install -y \
    rpi-update \
    chromium-browser \
    lsb-release && rm -rf /var/lib/apt/lists/*

RUN rpi-update

USER chromium