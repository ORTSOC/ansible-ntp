ansible-ntp
=========

Deploys an NTP server, a system clock syncing service.

Requirements
------------

- Debian 10
- sudo
- ssh

Role Variables
--------------

- `client_subnets`: A list of subnets that need permissions to access the NTP server, in addr+mask format.
  - `addr`: the address to mask
  - `mask`: the subnet mask

Example Playbook
----------------

Read traffic over 10.0.0.0/24 and 192.168.0.0/24 using the eth0 interface.

```yml
client_subnets:
  - addr: 192.168.1.0
  - mask: 255.255.255.0
```
License
-------

GPL3

Author Information
------------------

ORTSOC, Oregon State University
