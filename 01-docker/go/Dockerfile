FROM arm64v8/golang AS builder
WORKDIR /build
COPY . .
RUN go mod download
RUN go build -o ./main

FROM scratch
COPY --from=builder /build/main .
ENTRYPOINT ["./main"]