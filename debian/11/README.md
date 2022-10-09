# Debian 11

## Build

```
buildah build -f Containerfile -t custom-toolbox-debian-11
```

## Use

```shell
toolbox create --image localhost/custom-toolbox-debian-11:latest
```
