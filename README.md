# docker-v2ray-ws-tls-web
Docker Compose solution: v2ray + Caddy + openntpd.
Now works in [swarm mode](https://docs.docker.com/engine/swarm/).

**WARNING: `ntpd` service in this app would modify the time in host.**

## Usage

```
$ ./configure <UUID> <Host> <your_email>
$ docker stack deploy -c v2ray-stack.yml v2ray
```

And then connect to `https://<Host>:443` via vmess over wss with `path: "/filesync"`.

You may need to run `docker swarm init` before.

## Tips

You can run these commands in your local computer.
Just run
```sh
export DOCKER_HOST=ssh://<user>@<your.host>:22
```
before commands aforementioned.
