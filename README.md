# SNELL VPN SERVICE
## Command Install
### Version : 3
### Update Your Server
```
apt update && apt upgrade -y --fix-missing && apt install wget -y
```
### Install Snell
```
wget https://raw.githubusercontent.com/JAGOANNEON1986/SNELL/main/snell.sh && chmod +x snell.sh && ./snell.sh
```
### Untuk merubah PORT dan PSK
```
nano /etc/snell-server.conf
```

### Format Openclash
```
proxies:
  - name: Snellv3
    type: snell
    server: 128.199.79.115
    port: 443
    psk: jagoanneon
    version: '3'
    obfs-opts:
        mode: tls
        host: bug.com
    sni: bug.com
```
#### Root only set up to Version Linux Debian 10 buster
