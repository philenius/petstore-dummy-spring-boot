FROM golang:stretch
WORKDIR /go/src/app/
COPY app.go layout.html /go/src/app/
RUN go get && CGO_ENABLED=0 GOOS=linux go build -o app

FROM alpine
ENV MY_ENV_VAR=test
ENV SERVER_PORT=8081
RUN adduser -S user
USER user
WORKDIR /app/
COPY --from=0 /go/src/app/ .
EXPOSE 8081
CMD [ "./app" ]
