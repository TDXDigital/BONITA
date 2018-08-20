# Based on https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04

FROM ubuntu:16.04
RUN apt-get update
RUN apt-get install -y locales default-jre default-jdk
RUN apt-get upgrade -y

# Set the locale
RUN locale-gen en_CA.UTF-8
ENV LANG en_CA.UTF-8
ENV LANGUAGE en_CA:en
ENV LC_ALL en_CA.UTF-8

RUN /bin/bash echo JAVA_HOME="/usr/lib/jvm/java-8-oracle" >> /etc/environment
