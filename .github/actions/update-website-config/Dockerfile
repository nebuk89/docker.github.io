FROM golang:1.15

WORKDIR /src
COPY go.mod go.sum ./
RUN go mod download

COPY . .

RUN go build -o /bin/action

ENTRYPOINT ["/bin/action"]
