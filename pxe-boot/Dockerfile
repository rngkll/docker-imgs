FROM debian

MAINTAINER rngkll <alvarosb@gmail.com>

RUN apt-get -qy update

RUN apt-get install -y dnsmasq nginx

RUN mkdir -p /pxe/webroot
RUN mkdir -p /pxe/tftpboot/pxelinux.cfg

ADD nginx.conf /etc/nginx/sites-enabled/default
#ADD dnsmasq.conf /etc/dnsmasq.conf

EXPOSE 53/tcp 53/udp


	
