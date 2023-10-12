FROM golang:1.18-alpine

RUN mkdir /app

RUN addgroup -S informatika
RUN adduser -S -D -h /app yoyo informatika
RUN chown -R yoyo:informatika /app
USER yoyo

COPY main.go /app

EXPOSE 8080
CMD go run /app/main.go