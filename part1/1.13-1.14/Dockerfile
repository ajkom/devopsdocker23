FROM golang:1.16

#EXPOSE 8080

WORKDIR /usr/src/app

# Copy all of the source code
COPY . .

ENV REQUEST_ORIGIN=http://localhost:5001

RUN go build

CMD ["./server"]