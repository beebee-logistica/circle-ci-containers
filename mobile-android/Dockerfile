FROM circleci/android:api-27-node

ENV CI=true

USER root

RUN apt-get install -y gradle imagemagick \
    && npm i -g ionic@^4.5.0 cordova@^8.1.2 \
    && pip install awscli \
    && npm cache clean --force \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
