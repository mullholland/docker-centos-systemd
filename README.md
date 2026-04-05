CentOS Linux has been discontinued and is not safe to use anymore. [Read the information on upgrade and migration options](https://blog.centos.org/2023/04/end-dates-are-coming-for-centos-stream-8-and-centos-linux-7/).

Docker CentOS Systemd
=====================

This Dockerfile can build containers capable to use systemd.

Branches
--------

This repository has multiple tags that relate to CentOS versions.

|CentOS Version|Docker image tag      |
|--------------|----------------------|
| 9            | 9, stream9           |
| 10           | 10, stream10, latest |

Manually starting
-----------------

```shell
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  mullholland/docker-centos-systemd
```
