FROM alpine:latest

RUN apk update && apk add g++

WORKDIR /app

COPY app.cpp .

RUN g++ app.cpp -o app

EXPOSE 8080

CMD ["./app"]
