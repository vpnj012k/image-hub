FROM golang:1.15.11 as bd
WORKDIR /github.com/layer5io/dockercon-2020-api
ADD . .
RUN GOPROXY=direct GOSUMDB=off go build -a -o /api .
CMD ["/api"]