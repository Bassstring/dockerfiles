FROM alpine:latest

MAINTAINER Frank Roeder "piperly@icloud.com"

RUN apk --no-cache add imagemagick
WORKDIR /data

CMD [ "echo", "Usage: imagemagick convert foo.png foo.jpg \nAvailable commands: animate, compare, composite, conjure, convert, display, identify, import, mogrify, montage, stream" ]
