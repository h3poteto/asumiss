FROM node:5.12.0-slim

RUN useradd -m -s /bin/bash node
RUN echo 'node:password' | chpasswd
RUN mkdir -p /var/opt/app
RUN npm install -g npm-check-updates

USER node

WORKDIR /var/opt/app

ENV TZ Asia/Tokyo

CMD ["/bin/bash"]
