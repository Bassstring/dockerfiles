FROM alpine:latest

MAINTAINER Frank Roeder "piperly@icloud.com"

RUN set -xe \
    && apk add --no-cache curl python3 \
    && curl -sSL https://bootstrap.pypa.io/get-pip.py | python3

RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
RUN chmod a+rx /usr/local/bin/youtube-dl

WORKDIR /data

ENTRYPOINT ["python3", "/usr/local/bin/youtube-dl"]
CMD ["--help"]
