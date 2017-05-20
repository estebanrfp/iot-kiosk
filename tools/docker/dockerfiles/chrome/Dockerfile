FROM resin/rpi-raspbian:jessie
RUN useradd -ms /bin/bash chromium
RUN apt-get update && apt-get dist-upgrade && apt-get install -y \
    wget \
    curl \
    chromium-browser 
USER chromium