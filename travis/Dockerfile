FROM ubuntu:16.04

SHELL ["/bin/bash", "-x", "-c"]

RUN apt update && apt install -y ubuntu-dev-tools wget curl patchelf vim-common fuse libfuse2 libtool autoconf automake zlib1g-dev libjpeg-dev libpng-dev nano git 

ENV ARCH=aarch64
COPY entrypoint.sh /
SHELL ["/entrypoint.sh", "bash", "-x", "-c"]
ENTRYPOINT ["/entrypoint.sh"]
