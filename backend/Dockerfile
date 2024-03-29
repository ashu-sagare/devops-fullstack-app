FROM golang:1.19

WORKDIR /app

COPY . .

RUN go get ./...

ENV DB_HOST = ip-172.31.95.109
ENV DB_USER = admin
ENV DB_PASSWORD = admin
ENV DB_NAME = postgres-db-admin
ENV DB_PORT = 5432

ENV ALLOWED_ORIGINS = *

CMD ["go", "run", "main.go"]
