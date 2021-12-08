FROM ubuntu:18.04

RUN apt-get update && apt-get install -y \
curl

COPY web.sh .

CMD ./web.sh