# Automatic installation and configuration of WireGuard VPN server with web interface, node monitoring, with encryption on a free domain name

Only apt manager. For example Ubuntu, Debian

``I did a test run of the installation and configuration in Ubuntu 22.04, Ubuntu 24.04 and Debian 11, Debian 12``

``I recommend using it Debian. Requires 1 core, 1GB of RAM and 10-15GB of free disk space``

Thanks project: ...

Use the command to download and run the script:
```sh
apt-get update -qq && apt-get install -y git -qq && git clone -q https://github.com/sergeybezlepkin/vpn-wg-v14.git && cd vpn-wg-v14 && chmod +x menu.sh && ./menu.sh
```
