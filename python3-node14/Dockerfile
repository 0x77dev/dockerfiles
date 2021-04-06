FROM debian:buster

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && apt install -y curl
RUN curl -fsSL https://deb.nodesource.com/setup_14.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN apt update
RUN apt install -y nodejs yarn python3 python3-pip python3-setuptools
