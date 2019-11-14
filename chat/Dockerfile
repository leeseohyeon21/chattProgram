FROM golang:1.13.4

RUN mkdir /chat
WORKDIR /chat
COPY go.mod go.sum ./

RUN go mod download

COPY . .

RUN go build -o chat .

EXPOSE 8080

CMD ["./chat"]