FROM linuxserver/chromium:latest

RUN apt update
RUN apt install -y git nano
RUN npm install -g pnpm yarn

USER abc
RUN sudo npx puppeteer browsers install chrome@stable

USER root
RUN npx puppeteer browsers install chrome@stable
