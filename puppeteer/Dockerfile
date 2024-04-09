FROM linuxserver/chromium:latest

RUN sudo apt update
RUN sudo apt install -y git nano
RUN sudo npm install -g pnpm yarn
RUN yes | sudo npx puppeteer browsers install chrome@stable

WORKDIR /config

COPY ./real-estate-crawler.tgz ./real-estate-crawler.tgz

RUN tar -xvf ./real-estate-crawler.tgz && rm -rf ./real-estate-crawler.tgz
RUN sudo chmod +w /config/real-estate-crawler && sudo chmod +w /config/real-estate-crawler/* && sudo chmod +w /config/real-estate-crawler/**/*
