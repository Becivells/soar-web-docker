FROM golang:1.18-alpine as builder
ENV GOROOT="/usr/local/go"
ENV GOPATH="/root/go"
ENV PATH="${PATH}:${GOROOT}/bin"
ENV PATH="${PATH}:${GOPATH}/bin"

RUN apk update && apk --no-cache add gcc git make

RUN  git clone -b soar-web-go https://github.com/xiyangxixian/soar-web.git && cd   soar-web &&CGO_ENABLED=0 go build -o soar-web . && mv soar-web /root/

RUN mkdir  -p ${GOPATH}/src/github.com/XiaoMi/ && git clone -b dev https://github.com/XiaoMi/soar.git ${GOPATH}/src/github.com/XiaoMi/soar
RUN cd ${GOPATH}/src/github.com/XiaoMi/soar &&  CGO_ENABLED=0 make &&mv bin/soar /root/


FROM scratch
MAINTAINER  becivells <becivells@gmail.com>

COPY --from=builder /root/soar /soar-bin/soar
COPY --from=builder /root/soar-web /soar-web

WORKDIR  /
EXPOSE 5077
CMD ["/soar-web"]