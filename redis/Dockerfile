FROM redis:latest

MAINTAINER Dude Bub <dudebug@mail.com>

RUN apt-get update
RUN apt-get install -y gettext-base

COPY redis.conf /etc/redis/redis.conf.template
COPY start.sh /start.sh

ENTRYPOINT [ "/bin/bash", "/start.sh" ]
