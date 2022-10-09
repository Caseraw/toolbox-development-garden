# Ubuntu 22.04

## Build

```
buildah build -f Containerfile -t custom-toolbox-ubuntu-22.04
```

## Use

```shell
toolbox create --image localhost/custom-toolbox-ubuntu-22.04:latest
```
