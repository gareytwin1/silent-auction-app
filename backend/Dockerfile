# Start from the official Golang base image
FROM golang:1.21

WORKDIR /app

COPY . .

RUN go mod download
RUN go build -o auction-server ./cmd/auction-server

EXPOSE 8080

CMD ["./auction-server"]
