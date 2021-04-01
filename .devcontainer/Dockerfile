# Copyright (c) 2019 Futa HIRAKOBA
# Released under the MIT license
# https://opensource.org/licenses/MIT

FROM ubuntu:18.04

MAINTAINER Futa HIRAKOBA
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    xdvik-ja \ 
    evince \
    texlive-lang-cjk \
    latexmk \
    language-pack-ja \
    wget \
    xzdec \
    texlive-latex-extra \
    texlive-science \
RUN apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN tlmgr init-usertree
RUN kanji-config-updmap-sys ipaex

WORKDIR /workdir

VOLUME ["/workdir"]

# CMD ["bash"]

# FROM korosuke613/ubuntu-texlive-ja:latest
# MAINTAINER Futa HIRAKOBA

RUN apt-get update && apt-get install -y \
    git \
    cpanminus \
    texlive-extra-utils \
    make \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN cpanm Log::Log4perl Log::Dispatch::File YAML::Tiny File::HomeDir Unicode::GCString

RUN tlmgr option repository ftp://tug.org/historic/systems/texlive/2017/tlnet-final && \
    tlmgr install algorithms