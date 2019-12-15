FROM alpine:latest

MAINTAINER Frank Roeder "piperly@icloud.com"

RUN apk --no-cache add --update imagemagick \
      && mkdir -p /imgs

CMD [ "echo", "Usage: imagemagick convert /imgs/foo.png /imgs/foo.jpg \nAvailable commands: animate,compare,composite,conjure,convert,display,identify,import,mogrify,montage,stream" ]
