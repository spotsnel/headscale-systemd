Headscale (system container)
============================

Containerized version of headscale for use with podman

### Usage

#### Container creation
Start the system container. You can choose between the following options: [Debian](./#debian-based), [Fedora](./#fedora-based) or [RHEL UBI9](./#rhel-ubi9-based)

##### Debian-based
```
$ podman run -d --name=headscale \
        --hostname $HOSTNAME-headscale \
        --network=host --systemd=always \
        ghcr.io/spotsnel/headscale-systemd:latest
```

##### Fedora-based
```
$ podman run -d --name=headscale \
        --hostname $HOSTNAME-headscale \
        --network=host --systemd=always \
        ghcr.io/spotsnel/headscale-systemd/fedora:latest
```

##### RHEL UBI9-based
```
$ podman run -d --name=headscale \
        --hostname $HOSTNAME-headscale \
        --network=host --systemd=always \
        ghcr.io/spotsnel/headscale-systemd/ubi9:latest
```
