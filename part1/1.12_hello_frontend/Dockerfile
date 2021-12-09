FROM alpine:3.15

RUN apk update && apk add --update nodejs npm

COPY . .

WORKDIR /example-frontend

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD serve -s -l 5000 build