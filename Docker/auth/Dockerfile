FROM debian:13-slim

ENV DEBIAN_FRONTEND=noninteractive \
    TZ=UTC

RUN apt-get update && apt-get install -y --no-install-recommends \
    ca-certificates \
    curl \
    wget \
    gnupg \
    tzdata \
    build-essential \
    libace-dev \
    libtbb-dev \
    git \
    cmake \
    libmysql++-dev \
    openssl \
    libssl-dev \
    checkinstall \ 
    zlib1g-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /data

CMD ["realmd"]