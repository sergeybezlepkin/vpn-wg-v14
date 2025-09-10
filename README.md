# Automatic installation and configuration of WireGuard VPN server with web interface, node monitoring, with encryption on a free domain name

<div align="center">
  <img src="/docs/screenshots/wg-clear.png" width="50%" /> 
</div>

[WireGuard](https://www.wireguard.com/) is an extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec, while avoiding the massive headache. It intends to be considerably more performant than OpenVPN. WireGuard is designed as a general purpose VPN for running on embedded interfaces and super computers alike, fit for many different circumstances. Initially released for the Linux kernel, it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. It is currently under heavy development, but already it might be regarded as the most secure, easiest to use, and simplest VPN solution in the industry.

##
![menu.sh](/docs/screenshots/menu.PNG)
*Screenshot of running script
##

### What does the project do? 

This project is a collection of open technologies that allows both users and administrators to run their own VPN server using automation

### What problem does it solve?

Economy determines politics, law, ideology. Open news from the USA, Great Britain, Germany, Russia, France, show the crisis of these countries, the economic crisis of these countries pushes to adopt laws that limit the network space. Limiting the network space entails limiting technologies, limiting access to information. Information and technologies become private, limited, and this is a light breeze before a strong storm. Destroy it, use simple setup and installation of your private network in any country where you can buy a server, and get access to technologies and information. Be prepared for the storm

## Main features

-  Containers only (Docker)
-  Low resource consumption
-  Only 3 files to run
-  Installation and configuration via one point
-  Random VPN server port
-  Bridge network is used, after installation only ports 80 and 443 are open
-  Secure: Setting up encryption, proxying and default domain name
-  Configuring and setting default observability

### Thanks to these projects: [nginx-proxy](https://github.com/nginx-proxy/nginx-proxy), [letsencrypt](https://github.com/jwilder/docker-letsencrypt-nginx-proxy-companion), [wg-easy](https://github.com/wg-easy/wg-easy), [beszel](https://github.com/henrygd/beszel), [watchtower](https://github.com/containrrr/watchtower)

## Installation

Purchase a VPS or VDS server with the following minimum specifications: 1 CPU core, 1 GB RAM, and 15 GB of free disk space

Only distributions with the APT package manager (e.g. Ubuntu or Debian) are supported

``Installation and configuration tested on: Ubuntu 24.04, Ubuntu 22.04, Debian 12, Debian 11``

Launch terminal with superuser rights (root) and use the command to download and run the script:
```sh
curl -sL https://github.com/sergeybezlepkin/vpn-wg-v14/archive/refs/heads/main.tar.gz | tar xz && cd vpn-wg-v14-main && chmod +x menu.sh && ./menu.sh
```
If there is no curl and tar, we do the installation
```sh
apt update -qq && apt install -qq curl tar -y
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

After running the script, select the first item for installation and configuration. During the installation and configuration, the script will ask questions that you will need to answer.

The script also offers other actions:

-  Reset the password of the VPN server web panel (item 2)
-  Reset the password of the web monitoring panel (item 3)
-  Remind whether the server is running and what domain names are registered (item 4)
-  Configure notifications in Telegram in the monitoring system (item 5)

## [Download the client for your devices](https://www.wireguard.com/install/)

## License

This project uses the [MIT](https://github.com/sergeybezlepkin/vpn-wg-v14/blob/main/LICENSE)
