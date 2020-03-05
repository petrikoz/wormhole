# WormHole

Ansible's playbook for deploy personal server on Ubuntu.

## Soft

* [UFW](https://launchpad.net/ufw) — easy use firewall
* [Nginx](https://www.nginx.com/) — modern web server
* [acme.sh](https://acme.sh) — for free SSL via Let's Encrypt
* [uWSGI](https://uwsgi-docs.readthedocs.io/en/latest/) — for run sites on PHP and Python
* [Nextcloud](https://nextcloud.com/) — personal cloud service
* [Shadowsocks](https://shadowsocks.org) — a secure socks5 proxy (disabled by default)

## Install

1. Get root (or sudo) access to your server: use key-acces will be best choice
2. Change inventory with right server's IP
3. Run playbook: `ansible-playbook -i inventory wormhole.yml`
4. Or run only needed tags: `ansible-playbook -i inventory -t nextcloud -e "nextcloud_domain=cloud.example.com" wormhole.yml`
