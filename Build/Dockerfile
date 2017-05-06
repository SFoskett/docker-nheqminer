FROM ubuntu:16.04
MAINTAINER kmd.geek

RUN apt-get update && \
    apt-get install -y git cmake build-essential libboost-all-dev && \
    cd /tmp && \
    git clone -b Linux https://github.com/nicehash/nheqminer.git && \
    cd nheqminer && \
    git checkout -b 0.4b eb37570583ec639b4270e08b429ceb9bc6fe3077 \
    cd Linux_cmake/nheqminer_cpu_tromp && \
    cmake . && \
    make -j $(nproc) && \
    cp nheqminer_cpu_tromp   /nheqminer && \
    rm -rf /tmp/* && \
    chmod +x /nheqminer

WORKDIR /
CMD ["/nheqminer -h"]
