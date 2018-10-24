FROM simonbaeumer/goss-docker:0.3.6-gitcrypt
MAINTAINER Simon Bäumer

ENV OC_VERSION=v3.10.0

RUN wget https://github.com/openshift/origin/releases/download/${OC_VERSION}/openshift-origin-client-tools-${VERSION}-dd10d17-linux-64bit.tar.gz -O openshift.tar.gz
RUN tar -xf openshift.tar.xf
RUN mv openshift-origin-client-tools-${OC_VERSION}-dd10d17-linux-64bit/oc /usr/bin/oc
RUN mv openshift-origin-client-tools-${OC_VERSION}-dd10d17-linux-64bit/kubectl /usr/bin/kubectl

RUN chmod +x /usr/bin/oc
RUN chmod +x /usr/bin/kubectl