FROM alpine:latest

MAINTAINER Frank Roeder "piperly@icloud.com"

RUN apk --no-cache add ffmpeg

WORKDIR /data

ENTRYPOINT ["ffmpeg"]
CMD ["--help"]
