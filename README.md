Ubuntu Lucid (10.04) Dockerfile
===============================

tl;tr
-----


**Common:**
- [What is Scratch](https://github.com/docker-library/docs/tree/master/scratch)

**Ubuntu:**
- [Wiki](https://en.wikipedia.org/wiki/Ubuntu_(operating_system))
- [List of Ubuntu releases](https://en.wikipedia.org/wiki/List_of_Ubuntu_releases)
- [Docker Brew Ubuntu Core](https://github.com/tianon/docker-brew-ubuntu-core)
- [Lucid Dist](http://old-releases.ubuntu.com/ubuntu/dists/lucid/)

**Docker tools:**
- [mkimage](https://github.com/docker/docker/blob/master/contrib/mkimage.sh)
- [debootstrap](https://github.com/docker/docker/blob/master/contrib/mkimage/debootstrap)


How build core
--------------

Build command:

```bash
mkimage.sh -d . debootstrap --variant=minbase --components=main,universe --include=iproute,gpgv --arch=amd64 lucid http://old-releases.ubuntu.com/ubuntu
```
