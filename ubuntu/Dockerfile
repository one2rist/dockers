# syntax=docker/dockerfile:1

FROM ubuntu:20.04
ARG DEBIAN_FRONTEND=noninteractive
RUN apt update
RUN apt install -y git
RUN apt install -y vim-gtk3
RUN mkdir -p ~/.vim/autoload \
    && cd ~/.vim/autoload \
    && git clone https://github.com/tpope/vim-pathogen.git \
    && cp ./vim-pathogen/autoload/pathogen.vim .
RUN mkdir -p ~/.vim/bundle \
    && cd ~/.vim/bundle \
    && git clone https://github.com/scrooloose/nerdtree.git
COPY vimrc /etc/vim/vimrc
COPY vimrc /etc/vimrc
RUN apt install -y cmake
RUN apt install -y build-essential
