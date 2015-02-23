sysctl
======

Role which helps to manage `sysctl` configuration.


Example
-------

```
---

# Example of how to use the role
- hosts: myhost
  vars:
    sysctl_config:
      kernel.sysrq: 1
      net.ipv4.tcp_syncookies: 1
  roles:
    - sysctl
```


Role variables
--------------

List of variables used by the role:

```
# Default sysctl configuration
sysctl_config: {}

# Default sysctl.conf location
sysctl_config_location: /etc/sysctl.conf
```


License
-------

MIT


Author
------

Jiri Tyr
