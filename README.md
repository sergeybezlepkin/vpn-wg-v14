# Automatic installation and configuration of WireGuard VPN server with web interface, node monitoring, with encryption on a free domain name

## What does the project do? What problem does it solve?

This project is a collection of open technologies that allows both users and administrators to run their own VPN server using automation

## Main features

-  Containers only (Docker)
-  Low resource consumption
-  Installation and configuration via one point
-  Secure: Setting up encryption, proxying and default domain name
-  Configuring and Setting Default Observability

Thanks to these projects: [nginx-proxy](https://github.com/nginx-proxy/nginx-proxy), [letsencrypt](https://github.com/jwilder/docker-letsencrypt-nginx-proxy-companion), [wg-easy](https://github.com/wg-easy/wg-easy), [beszel](https://github.com/henrygd/beszel), [watchtower](https://github.com/containrrr/watchtower)


## Installation and launch

Purchase a VPS or VDS server with the following minimum specifications: 1 CPU core, 1 GB RAM, and 15 GB of free disk space

``OS requirements: Only distributions with the APT package manager (e.g. Ubuntu or Debian) are supported``

``Installation and configuration tested on: Ubuntu 24.04, Ubuntu 22.04, Debian 12, Debian 11``

Launch terminal with superuser rights (root) and use the command to download and run the script:
```sh
curl -sL https://github.com/sergeybezlepkin/vpn-wg-v14/archive/refs/heads/main.tar.gz | tar xz && cd vpn-wg-v14-main && chmod +x menu.sh && ./menu.sh
```
If there is no curl, we do the installation
```sh
apt update -qq && apt install -qq curl -y
```

or

Clone the repository
```sh
git clone https://github.com/sergeybezlepkin/vpn-wg-v14.git
```
We go to the catalog
```sh
cd vpn-wg-v14.git
```
Make the menu.sh file executable and run it
```sh
chmod +x menu.sh && ./menu.sh
```
---
**Usage:**
Enter a number (1–6) to select an option.
