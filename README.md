# docker-v2ray-ws-tls-web
Docker composer solution: v2ray + Caddy.

## Usage

```
$ ./configure <UUID> <Host>
$ sudo docker-compose up -d
```

Then connect to https://<Host>:443 via vmess over ws.
