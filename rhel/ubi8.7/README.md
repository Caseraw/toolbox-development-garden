# RHEL UBI8.7

## Login

```
buildah login registry.redhat.io
```

## Build

```
buildah build -f Containerfile -t custom-toolbox-rhel-ubi8.7
```

## Use

```shell
toolbox create --image localhost/custom-toolbox-rhel-ubi8.7:latest
```
