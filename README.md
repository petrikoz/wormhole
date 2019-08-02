# WormHole

Ansible's playbook for deploy personal server.

## Soft

* Shadowsocks - for encrypted access to remote server
* Dnsmasq - for hidden personal name resolve
* NextCloud - replace for most social services
* Acme.sh - for free SSL via Let's Encrypt

## Install

1. Get root (or sudo) access to your server: use key-acces will be best choice
2. Change inventory with right server's IP
3. Run playbook: `ansible-playbook -i inventory wormhole.yml`
4. Or run only needed tags: ex. `ansible-playbook -i inventory -t common -e "common_hostname=wormhole" wormhole.yml`