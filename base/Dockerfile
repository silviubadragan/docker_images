FROM ubuntu:latest

RUN apt-get update && apt-get install -y --no-install-recommends \
    mc \
    fish \
    git \
    curl \
    wget \
    tmux \
    vim

RUN apt-get install -y --no-install-recommends \
    ca-certificates

WORKDIR /home/root

RUN curl -L https://get.oh-my.fish > install_omf \ 
    && chmod +x install_omf \
    && fish -c './install_omf --noninteractive -y' \
    && rm -rf ./install_omf

ENTRYPOINT [ "/usr/bin/env", "fish" ]
CMD []

