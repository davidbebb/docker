FROM ubuntu:15.10
RUN apt-get -y update
RUN apt-get -y update
RUN apt-get install -y make gcc libkrb5-dev g++ python openssh-client curl rsync git
RUN curl -sL https://deb.nodesource.com/setup_4.x | bash -
RUN apt-get install -y nodejs default-jre default-jdk mongodb
RUN npm install -g selenium-standalone@latest
RUN npm install -g phantomjs
RUN selenium-standalone install

