# Install a Dante Server in docker

[Dante](https://www.inet.no/dante/) is a product developed by Inferno Nettverk A/S. It consists of a SOCKS server and a SOCKS client, implementing RFC 1928 and related standards. It is a flexible product that can be used to provide convenient and secure network connectivity.

Using a [LinuxServer.io](https://www.linuxserver.io/) base Alpine image, their [Universal Package Installer](https://github.com/linuxserver/docker-mods/tree/universal-package-install) to install Dante from the Alpine repository, and finally their ability to [run custom services](https://www.linuxserver.io/blog/2019-09-14-customizing-our-containers) with just a docker-compose file and a single file `dante` contained in this repository means an easy to use versatile SOCKS proxy with no maintenance support other than occasionally incrementing th base image version tag (currently on 3.20).

After the first run just edit `/config/sockd.conf` to configure dante to your liking.