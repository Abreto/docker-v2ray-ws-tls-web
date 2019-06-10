# docker-v2ray-ws-tls-web
Docker Compose solution: v2ray + Caddy + openntpd.

**WARNING: `ntpd` service in this app would modify the time in host.**

## Usage

```
$ ./configure <UUID> <Host>
$ sudo docker-compose up -d
```

Then connect to `https://<Host>:443` via vmess over wss with `path: "/filesync"`.
