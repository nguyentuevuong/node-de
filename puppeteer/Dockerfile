FROM linuxserver/chromium:latest

USER abc

RUN sudo apt update
RUN sudo apt install -y git nano
RUN sudo npm install -g pnpm yarn
RUN sudo npx puppeteer browsers install chrome@stable

WORKDIR /real-estate-crawler