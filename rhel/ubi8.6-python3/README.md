# RHEL UBI8.6 - Python3

## Login

```
buildah login registry.redhat.io
```

## Build

```
buildah build -f Containerfile -t custom-toolbox-rhel-ubi8.6-python3
```

## Use

```shell
toolbox create --image localhost/custom-toolbox-rhel-ubi8.6-python3:latest
```
