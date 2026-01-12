# docker/Dockerfile
FROM ubuntu:22.04

ENV TZ=Asia/Tokyo
ENV DEBIAN_FRONTEND=noninteractive

# 最低限のツールだけ
RUN apt-get update && apt-get install -y \
    sudo \
    vim \
    curl \
    iputils-ping \
    net-tools \
    wget \
    build-essential \
    libpcre3-dev \
    zlib1g-dev \
    libssl-dev \
    tar \
 && rm -rf /var/lib/apt/lists/*

# 上に混ぜれるなら混ぜて
 RUN apt update

 RUN apt install -y iproute2

# コンテナ起動時に bash
CMD ["bash"]
