## Nairobi GNU/Linux Users Group Telegram - IRC Gateway

This repository contains playbooks for provisioning the NairobiLUG's Telegram ↔ IRC gateway.


### Running the Playbooks

You'll need to obtain the password file used to decryp the vaults in this repo (you can get that from the mailing list). Make sure you symlink a hosts file with the `gateways` group to `inventories/production/hosts`, then run:

```
cd ansible
ansible-playbook --vault-password-file=[path to password file] -i inventories/production/hosts gateways.yml
```


### Telegram Commands

Here's a list of commands you can run while on the NairobiLUG Telegram Group:

 - `/command`: Send IRC msg without nick prefix
 - `/me`: Send action message
 - `/names`: List users on IRC
 - `/topic`: Get IRC channel topic
 - `/version`: Show version of teleirc
