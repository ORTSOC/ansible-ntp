# ansible-ntp
ORTSOC Infra Role: NTP Server

# Variables

* `client_subnets`: All of the subnets that need permissions to access the NTP server. Example:
  ```yml
  client_subnets:
    - addr: 192.168.1.0
    - mask: 255.255.255.0
  ```
