FROM circleci/android:api-28-node

ENV CI=true

USER root

RUN apt-get update \
    && apt-get install -y gradle imagemagick \
    && npm i -g ionic@^5.4.2 cordova@^9.0.0 native-run@^0.2.8 \
    && npm i -g --unsafe-perm cordova-res@^0.5.2 \
    && pip install awscli \ 
    && npm cache clean --force \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
