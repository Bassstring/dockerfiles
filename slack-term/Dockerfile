FROM golang:alpine

MAINTAINER Frank Roeder "piperly@icloud.com"

RUN apk --no-cache add git
RUN set -x && go get -u github.com/erroneousboat/slack-term && \
      cd $GOPATH/src/github.com/erroneousboat/slack-term && \
      go install .

ENTRYPOINT stty cols 25 && slack-term
