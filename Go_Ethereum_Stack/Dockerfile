FROM golang:1.13-alpine

# install build tools 
RUN apk add --no-cache make gcc musl-dev linux-headers git
# clone ethereum tools
RUN go get -d github.com/ethereum/go-ethereum
# Change WorkDir
WORKDIR /go/src/github.com/ethereum/go-ethereum
# install
RUN go install ./...

WORKDIR /root/
