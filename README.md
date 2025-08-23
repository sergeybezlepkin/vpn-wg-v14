# Automatic installation and configuration of WireGuard VPN server with web interface, node monitoring, with encryption on a free domain name

Only apt manager. For example Ubuntu, Debian

``I did a test run of the installation and configuration in Ubuntu 24.04, Ubuntu 22.04, and Debian 12, Debian 11``

``I recommend using it Debian. Requires 1 core, 1GB of RAM and 15GB of free disk space``

Thanks projects: [nginx-proxy](https://github.com/nginx-proxy/nginx-proxy), [letsencrypt](https://github.com/jwilder/docker-letsencrypt-nginx-proxy-companion), [wg-easy](https://github.com/wg-easy/wg-easy), [beszel](https://github.com/henrygd/beszel), [watchtower](https://github.com/containrrr/watchtower) 

Use the command to download and run the script:
```sh
curl -sL https://github.com/sergeybezlepkin/vpn-wg-v14/archive/refs/heads/main.tar.gz | tar xz && cd vpn-wg-v14-main && chmod +x menu.sh && ./menu.sh
```
