FROM resin/rpi-raspbian:jessie
RUN useradd -ms /bin/bash chromium
RUN sudo apt-get update && apt-get install -y \
    wget \
    ttf-mscorefonts-installer \
    chromium-browser 

USER chromium