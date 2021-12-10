FROM alpine:3.15

EXPOSE 3000

RUN apk update && apk add --update nodejs npm

COPY /homework /bin/usr/app

WORKDIR /bin/usr/app

RUN npm install -g serve

CMD serve -s -l 3000 build