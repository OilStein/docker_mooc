FROM golang:alpine3.15

EXPOSE 8080

COPY . .

RUN cd example-backend && go build

CMD cd example-backend && REQUEST_ORIGIN=http://localhost:5000 ./server