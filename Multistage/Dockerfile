FROM golang:1.15
WORKDIR /app
COPY ./hello.go /app
RUN go build -o goapp
ENTRYPOINT ["/app/goapp"]
