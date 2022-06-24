FROM golang:1.16
WORKDIR /usr/src/app/
COPY . .
COPY go.mod ./
COPY go.sum ./
RUN go mod download
RUN go build 
ENV REQUEST_ORIGIN http://localhost:5000
#EXPOSE 8080
CMD ["./server"]
