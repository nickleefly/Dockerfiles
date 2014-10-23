FROM ubuntu

RUN apt-get update -y && \
  apt-get -y upgrade && \
  apt-get install --no-install-recommends -y -q curl python && \
  apt-get install -y build-essential && \
  apt-get install -y software-properties-common git ca-certificates && \
  rm -rf /var/lib/apt/lists/*

RUN mkdir /nodejs && curl http://nodejs.org/dist/v0.10.32/node-v0.10.32-linux-x64.tar.gz | tar xvzf - -C /nodejs --strip-components=1

ENV PATH $PATH:/nodejs/bin
