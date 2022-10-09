# Toolbox development garden

Pick a distribution, add your custom stuff and build your own toolbox image!

## Requirements

On you host computer the following packages are required.

```shell
sudo dnf install -y \
podman \
toolbox \
buildah \
skopeo
```

## Index of toolbox images

- [Fedora](fedora/)
    - [36](fedora/36/)
    - [37](fedora/37/)
- [RHEL](rhel/)
    - [ubi8.6](rhel/ubi8.6/)
- [Debian](debian/)
    - [11](debian/11/)
- [Ubuntu](ubuntu/)
    - [22.04](ubuntu/22.04/)

## Toolbox custom images

Check out [official fedora examples](https://github.com/containers/toolbox/tree/main/images/fedora) to get inspired in building toolbox images.

Create a custom image:

```shell
buildah build -f Containerfile -t my-custom-image:123
```

Use custom image with toolbox:

```shell
toolbox create --image localhost/my-custom-image:123:latest
```

## Toolbox run 

```
toolbox run my-custom-image:123:latest
```

## Resources

### Toolbox

- https://containertoolbx.org/
- https://containertoolbx.org/install/
- https://containertoolbx.org/distros/
- https://github.com/containers/toolbox
- https://github.com/containers/toolbox/tree/main/images
- https://docs.fedoraproject.org/en-US/fedora-silverblue/toolbox/

### Podman
- https://podman.io/
- https://podman.io/getting-started/installation
- https://podman-desktop.io/
- https://podman-desktop.io/downloads/Linux
- https://flathub.org/apps/details/io.podman_desktop.PodmanDesktop

### Skopeo

- https://github.com/containers/skopeo


### Buildah

- https://buildah.io/
- https://github.com/containers/buildah/blob/main/install.md
- https://github.com/containers/buildah/tree/main/docs/tutorials
