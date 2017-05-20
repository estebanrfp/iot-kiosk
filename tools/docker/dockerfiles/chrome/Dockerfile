FROM resin/rpi-raspbian:jessie
RUN useradd -ms /bin/bash chromium
RUN apt-get update && apt-get dist-upgrade && apt-get install -y \
    wget \
    curl \
    rpi-update \
    git-core \
    chromium-browser \
    xorg \
    lsb-release && rm -rf /var/lib/apt/lists/*

RUN rpi-update

USER chromium