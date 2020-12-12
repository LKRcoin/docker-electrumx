# docker-electrumx

> Run an Electrum server with one command

## Build

```
docker build -t electrumx-lkrcoin:latest .
```

## Usage

```
docker run \
  --name=electrumx-lkr -d  \
  -v /data/electrumx-data:/data  \
  -e DAEMON_URL=http://user:pass@host:port \
  -e COIN=Lkrcoin \
  -p 30001:30001 -p 30002:30002 electrumx-lkrcoin:latest
```

## Show logs

```

docker logs -f electrumx-lkr

```
