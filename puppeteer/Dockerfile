FROM linuxserver/chromium:latest

RUN apt update
RUN apt install -y git nano
RUN npm install -g pnpm yarn
RUN npx puppeteer browsers install chrome@stable
