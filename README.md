Hosts
=========

This role manages /etc/hosts and /etc/hostname. The files are managed with a
template.

## Hosts

Create a dynamic hosts file from the repository. Useful for a 
cluster which need to talk to eachother over the local network
using a hostname.

Passing in custom entries is allowed using the *hosts_custom_hosts* 
variable.

Make sure per hosts the ```hosts_ansible_eth``` variable exists. This 
should contain the interface to use, for exaple ```ansible_eth1```.

## Hostname

The hostname is set permanenty through the hostname file and directly 
using the command.