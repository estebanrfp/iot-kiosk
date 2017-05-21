#FROM resin/rpi-raspbian:wheezy
FROM armhf/alpine

RUN sudo apt-get update && sudo apt-get install --no-install-recommends -y \
	openbox \
    xserver-xorg \
    xinit \
    xserver-xorg-video-fbdev

COPY x.sh /

RUN chmod 700 /x.sh

CMD ["/x.sh"]