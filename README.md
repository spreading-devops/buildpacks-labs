# Buildpacks

### Environment
```
Windows 11 Pro 22H2 (OS Build 22621.1848)
WSL2 + Ubuntu 22.04.2 LTS
Docker Desktop 4.20.1
pack 0.29.0
```

### List the base images that Pack suggest you use
```bash
$ pack builder suggest
```

### Create a new Container image using one of suggest base images
```bash
$ pack build nodejs-app --builder paketobuildpacks/builder:base
```

### List Container Images
```bash
$ docker image ls
```

### Running the new Container Image
```bash
$ docker run --rm -p 3000:3000 nodejs-app
```

