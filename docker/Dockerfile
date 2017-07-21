FROM ubuntu
MAINTAINER erik.kugel@gmail.com
EXPOSE 123
RUN apt-get update && apt-get install -y ntp
ADD ntp.conf /ntp.conf
ENTRYPOINT ntpd --nofork --config /ntp.conf
