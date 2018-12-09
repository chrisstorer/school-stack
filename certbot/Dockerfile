FROM ubuntu:18.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update
RUN apt-get install -y software-properties-common
RUN add-apt-repository universe
RUN add-apt-repository ppa:certbot/certbot
RUN apt-get update
RUN apt-get install -y python-certbot-apache

CMD /bin/bash
#certbot --text --agree-tos --email spam_bob@live.co.uk -d idev.chrisstorer.co.uk --manual --preferred-challenges dns --expand --renew-by-default  --manual-public-ip-logging-ok certonly
