FROM golang:1.16.13 as bd
WORKDIR /github.com/layer5io/dockercon-2020-api
ADD . .
RUN GOPROXY=direct GOSUMDB=off go build -a -o /api .
CMD ["/api"]