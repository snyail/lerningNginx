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
 && rm -rf /var/lib/apt/lists/*

# コンテナ起動時に bash
CMD ["bash"]
