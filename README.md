# WormHole

Ansible's playbook for deploy personal server.

## Soft

* Acme.sh — for free SSL via Let's Encrypt
* Dnsmasq — for hidden personal name resolve
* Nextcloud — replace for most social services
* Shadowsocks — for encrypted access to remote server
* uWSGI — for run projects on PHP and Pyhton

## Install

1. Get root (or sudo) access to your server: use key-acces will be best choice
2. Change inventory with right server's IP
3. Run playbook: `ansible-playbook -i inventory wormhole.yml`
4. Or run only needed tags: `ansible-playbook -i inventory -t nextcloud -e "nextcloud_domain=cloud.example.com" wormhole.yml`
