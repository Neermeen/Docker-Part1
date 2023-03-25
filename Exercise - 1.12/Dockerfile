FROM ubuntu:20.04

WORKDIR /usr/src/

COPY . .

RUN apt-get update && apt install -y curl

RUN curl -sL [https://deb.nodesource.com/setup_16.x](https://deb.nodesource.com/setup_16.x) | bash

RUN apt install -y nodejs
RUN npm install
RUN npm run build

RUN npm install -g serve

EXPOSE 5000

CMD ["serve","-s","-l","5000","build"]
