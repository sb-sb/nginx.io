## Supported OS

* Debian 9 Stretch
* Debian 10 Buster
* Debian 11 Bullseye
* Ubuntu 18.04 Bionic
* Ubuntu 20.04 Focal

## Install via DEB

```bash
apt install apt-transport-https lsb-release ca-certificates curl gnupg -y
curl https://mirrors.xtom.com/sb/nginx/public.key | apt-key add -
echo "deb https://mirrors.xtom.com/sb/nginx/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/sb-nginx.list
apt update
apt install nginx-extras
```

## Install from Docker

Check [Docker image for sb-nginx](https://github.com/brentybh/docker-sb-nginx)

## Install for End-of-life OS

We do not provide any further support for end-of-life OS such as Debian 8 Jessie, Ubuntu 19.04 Disco, but you can try it at your own risk

```bash
apt install apt-transport-https lsb-release ca-certificates curl gnupg -y
curl https://mirrors.xtom.nl/sb/nginx/public-rsa.key | apt-key add -
echo "deb https://mirrors.xtom.com/sb/nginx/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/sb-nginx.list
apt update
apt install nginx-extras
```