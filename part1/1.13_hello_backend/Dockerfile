FROM golang:alpine3.15

COPY . .

RUN cd example-backend && go build

CMD cd example-backend && ./server