FROM node:8-slim

ENV CI=true

RUN apt-get update \
    && apt-get install -y python-pip imagemagick \
    && npm i -g ionic@^4.5.0 cordova@^8.1.2 \
    && pip install awscli \
    && npm cache clean --force \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
