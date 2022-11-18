FROM caddy:2.6.2-builder-alpine AS builder

RUN xcaddy build         --with github.com/gamalan/caddy-tlsredis@v0.2.9

#FROM caddy:2.6.2-alpine
FROM alpine:3.16.2 AS runner

COPY . /CaterZen/Build/Caddy
COPY --from=builder /usr/bin/caddy /CaterZen/Build/Caddy/caddy 

CMD ["/CaterZen/Build/Caddy/caddy", "run", "--config", "/CaterZen/Build/Caddy/caddy.json"]

