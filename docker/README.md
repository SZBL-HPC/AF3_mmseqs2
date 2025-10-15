## Build

```bash
cd ./docker
podman build -t af3mmseqs2 -f docker/Dockerfile ..
# The .. make this work.

podman save localhost/af3mmseqs2:new -o p.tar
apptainer build af3mmseqs2new.simg docker-archive://p.tar
```

