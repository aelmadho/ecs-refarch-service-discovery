FROM golang

RUN go get github.com/goji/httpauth && go get github.com/gorilla/mux

COPY src /go/src/github.com/awslabs/ECS-refarch-service-discovery/goodreads

RUN go install github.com/awslabs/ECS-refarch-service-discovery/goodreads

EXPOSE 80

ENTRYPOINT ["/go/bin/goodreads"]
