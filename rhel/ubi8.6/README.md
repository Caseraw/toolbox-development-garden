# RHEL UBI8.6

## Login

```
buildah login registry.redhat.io
```

## Build

```
buildah build -f Containerfile -t custom-toolbox-rhel-ubi8.6
```

## Use

```shell
toolbox create --image localhost/custom-toolbox-rhel-ubi8.6:latest
```
