FROM ghcr.io/danussi/steamcmd:main

USER root

RUN pacman -Syu --needed --noconfirm  \
    bash  \
    coreutils  \
    findutils  \
    perl  \
    rsync \
    sed \
    tar \
    curl \
    lsof \
    lib32-gcc-libs \
    bzip2 \
    nano

RUN git clone --depth 1 -b master https://github.com/arkmanager/ark-server-tools.git && \
    cd ark-server-tools/tools && \
    bash install.sh ark && \
    rm -rf /home/ark/ark-server-tools


USER ark
CMD ["/usr/local/bin/arkmanager"]