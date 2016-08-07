FROM node:5.12.0-slim

ENV TZ Asia/Tokyo

RUN mkdir -p /var/opt/app

WORKDIR /var/opt/app

COPY . /var/opt/app

RUN npm install


CMD bin/hubot -a slack
