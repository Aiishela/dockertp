FROM ubuntu:latest
RUN apt-get update && apt-get install -y golang
ADD static ./static
ADD dispatcher.go ./dispatcher.go

RUN go build dispatcher.go 
CMD ["./dispatcher"]
