# Squid Proxy Installer


Auto install Squid 3 proxy on following linux OS.

* Ubuntu 14.04, 16.04, 18.04, 20.04, 22.04
* Debian 8, 9, 10
* CentOS 7, 8


## Install Squid

To install, run the script

```
wget https://raw.githubusercontent.com/serverok/squid-proxy-installer/master/squid3-install.sh -O squid3-install.sh
```
```
sudo bash squid3-install.sh
```


To create users, run

```
sudo /usr/bin/htpasswd -b -c /etc/squid/passwd root root
```

Change Squid https
```
wget -O /etc/squid/squid.conf https://raw.githubusercontent.com/gilangkurniiawant/squid/master/squid.conf  /etc/squid
```

Reload squid proxy

```
sudo systemctl reload squid
```

