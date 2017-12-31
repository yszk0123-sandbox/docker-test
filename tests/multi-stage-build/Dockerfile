FROM golang:alpine AS build
COPY . /work
WORKDIR /work
RUN go build -o hello main.go

FROM busybox
COPY foo.txt /app/foo.txt
WORKDIR /app
RUN ls -la
COPY --from=build /work/hello /usr/local/bin/hello
ENTRYPOINT ["/usr/local/bin/hello"]
