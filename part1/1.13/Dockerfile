FROM golang:1.16

#EXPOSE 8080

WORKDIR /usr/src/app

# Copy all of the source code
COPY . .

RUN go build

ENV REQUEST_ORIGIN=http://localhost:8080/ping

CMD ["./server"]
