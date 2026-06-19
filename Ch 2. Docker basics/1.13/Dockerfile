FROM golang:1.16

WORKDIR /app

COPY example-backend .

RUN go build

ENV PORT=8080

EXPOSE 8080

ARG REQUEST_ORIGIN=http://localhost:5001
ENV REQUEST_ORIGIN=$REQUEST_ORIGIN

CMD ["./server"]