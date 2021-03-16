Debian Systemd Container Image
=====================

This Containerfile can build containers capable to use systemd.

[![debian build status](https://quay.io/repository/ucomesdag/debian/status "Container Repository on Quay")](https://quay.io/repository/ucomesdag/debian)

Branches
--------

This repository has multiple branches that relate to Debian versions.

|Branch  |Debian Version    |Container image tag|
|--------|------------------|-------------------|
|buster  |buster (10)       |buster             |
|main    |bullseye (11)     |latest             |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
podman run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  quay.io/ucomesdag/debian:buster
```
