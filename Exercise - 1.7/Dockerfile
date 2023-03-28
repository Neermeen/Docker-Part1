FROM ubuntu:20.04

WORKDIR /usr/src/app

RUN apt -y update
RUN apt install -y curl

COPY new.sh .

RUN chmod +x new.sh

CMD ./new.sh
