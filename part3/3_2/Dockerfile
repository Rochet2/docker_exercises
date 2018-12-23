FROM alpine:3.8

RUN apk add --no-cache \
    bash \
    ffmpeg \
    gcc \
    libxml2-dev \
    libxslt-dev \
    make \
    musl-dev \
    py-crypto \
    py-lxml \
    py-pip \
    py-setuptools \
    python \
    python2-dev \
    tar \
    wget

RUN pip install -U pip setuptools youtube_dl yle-dl

WORKDIR /out
ENTRYPOINT ["yle-dl"]
