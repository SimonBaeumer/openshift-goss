FROM sselzer/openshift-cli-gitcrypt
MAINTAINER Simon Bäumer

ENV GOSS_FILES_STRATEGY=cp
ENV GOSS_VERSION=v0.3.6
ENV GOSS_PATH=/usr/bin/goss

RUN apk update
RUN apk add wget

RUN wget https://github.com/aelsabbahy/goss/releases/download/${GOSS_VERSION}/goss-linux-amd64 -O /usr/bin/goss
RUN chmod +x /usr/bin/goss

RUN wget https://github.com/aelsabbahy/goss/releases/download/${GOSS_VERSION}/dgoss -O /usr/bin/dgoss
RUN chmod +x /usr/bin/dgoss

RUN mkdir /goss

VOLUME /goss
WORKDIR /goss
