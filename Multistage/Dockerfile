FROM golang:alpine
WORKDIR /app
COPY ./hello.go /app
RUN cd /app && go build -o goapp
ENTRYPOINT ["/app/goapp"]
