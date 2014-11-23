# docker-quassel-core

[Quassel IRC](http://quassel-irc.org/) is a modern, cross-platform, distributed IRC program,
where multiple clients can attach to and detach from a central core.
This is a [docker](https://www.docker.io) image that eases setup.

## Usage

This docker image is available as a [trusted build on the docker
index](https://registry.hub.docker.com/u/asmaps/quassel-core/),
so using it is as simple as running:

```bash
docker run -p 4242:4242 -v /opt/quassel:/var/lib/quassel asmaps/quassel-core
```

Running this command for the first time will download the image automatically.
Further runs will be immediate, as the image will be cached locally.  
The configdir will be mounted and persisted in the hosts /opt/quassel directory.
