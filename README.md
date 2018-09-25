# Docker os images 

## Intended use
* for air gapped systems we need to import these images since there's no "image: xxxx" possible

## How images were obtained

```
$ docker pull busybox
$ docker save busybox -o busybox.tar

$ docker pull phusion/baseimage
$ docker save phusion/baseimage -o baseimage.tar

$ docker pull blacklabelops/alpine
$ docker save blacklabelops/alpine -o blacklabel-alpine.tar

$ docker pull blacklabelops/ubuntu
$ docker save blacklabelops/ubuntu -o blacklabel-ubuntu.tar

$ gzip *

```


