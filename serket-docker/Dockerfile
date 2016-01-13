FROM ubuntu:15.10
RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get -y install curl
RUN curl -sL https://deb.nodesource.com/setup_4.x | bash -
RUN apt-get install -y nodejs default-jre default-jdk mongodb
RUN npm install -g selenium-standalone@latest
RUN npm install -g phantomjs
RUN selenium-standalone install
