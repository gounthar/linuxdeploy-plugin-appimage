FROM ubuntu:18.04

SHELL ["/bin/bash", "-x", "-c"]

RUN apt install -y devtoolset-7 wget curl patchelf vim-common fuse libfuse2 libtool autoconf automake zlib-devel libjpeg-devel libpng-devel nano git 

ENV ARCH=aarch64
COPY entrypoint.sh /
SHELL ["/entrypoint.sh", "bash", "-x", "-c"]
ENTRYPOINT ["/entrypoint.sh"]
