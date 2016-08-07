FROM node:5.12.0-slim

RUN apt-get update && \
    apt-get install -y python \
    build-essential && \
    rm -rf /var/cache/apt/archives/* /var/lib/apt/lists/*


RUN useradd -m -s /bin/bash node
RUN echo 'node:password' | chpasswd
RUN mkdir -p /var/opt/app

USER node

WORKDIR /var/opt/app

ENV TZ Asia/Tokyo

CMD ["/bin/bash"]
