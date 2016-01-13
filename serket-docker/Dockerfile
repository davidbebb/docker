FROM ubuntu:15.10

RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get install -y wget
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub |  apt-key add -
RUN sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
RUN apt-get -y update
RUN apt-get -y install curl google-chrome-stable
RUN curl -sL https://deb.nodesource.com/setup_4.x | bash -
RUN apt-get install -y nodejs default-jre default-jdk mongodb
RUN npm install -g selenium-standalone@latest
RUN selenium-standalone install --drivers.chrome.version=2.20 --drivers.chrome.baseURL=https://chromedriver.storage.googleapis.com
RUN apt-get -y install xvfb
CMD xvfb-run --server-args='-screen 10, 1024x768x16' google-chrome -start-maximized > /dev/null &
