FROM golang:alpine
WORKDIR /app
COPY . /app
RUN cd /app && go build -o goapp
ENTRYPOINT ["/app/goapp"]
