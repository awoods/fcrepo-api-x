FROM alpine:3.4
ENV GOPATH=/go \
    PATH=/go/bin:/usr/local/go/bin:$PATH

WORKDIR $GOPATH

#RUN echo "@edge http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories && \
RUN    apk update && \
    mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH" && \
    apk add --no-cache build-base go git openssl-dev luajit-dev 
