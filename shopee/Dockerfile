FROM golang:1.8.0

RUN apt-get update && apt-get install -y --no-install-recommends \
        libpng-dev \
    && rm -rf /var/lib/apt/lists/*

RUN go get -u github.com/pquerna/ffjson
RUN go install github.com/pquerna/ffjson

ENV PATH $GOPATH/bin:$PATH

CMD cd /go/src/git.garena.com/shopee-server
