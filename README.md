# crux-ports-efikamx-arm

CRUX-ARM ports overlay for Genesi EfikaMX

To use these ports, download the `efikamx-arm.httpup` file to `/etc/ports`:
```
$ sudo curl -o /etc/ports/efikamx-arm.httpup \
    https://raw.githubusercontent.com/crux-arm/crux-ports-efikamx-arm/3.8/efikamx-arm.httpup
$ sudo ports -u efikamx-arm
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/efikamx-arm
prtdir /usr/ports/core-arm
prtdir /usr/ports/opt-arm
prtdir /usr/ports/xorg-arm
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```
