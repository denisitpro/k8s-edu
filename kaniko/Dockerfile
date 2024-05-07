FROM golang:latest AS sources

WORKDIR /opt/app/
RUN git clone https://github.com/denisitpro/go-example-apps.git
RUN cd go-example-apps && go build main.go

FROM ubuntu:latest
WORKDIR /opt/app/

COPY --from=sources /opt/app/go-example-apps/main /opt/app/go-app

EXPOSE 8082
CMD ["./go-app"]
