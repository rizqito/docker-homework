FROM golang:alpine AS builder
WORKDIR /app-be
COPY . .
RUN go build -o /go-server

FROM alpine:latest AS runner
ENV DB_USER="root"
ENV DB_PASS=""
EXPOSE 8080
COPY --from=builder /go-server /go-server
CMD ["/go-server"]