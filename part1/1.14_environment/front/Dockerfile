FROM alpine:3.15

EXPOSE 3000

RUN apk update && apk add --update nodejs npm

COPY . .

WORKDIR /example-frontend

RUN npm install

RUN REACT_APP_BACKEND_URL=http://localhost:8080 npm run build

RUN npm install -g serve

CMD serve -s -l 5000 build