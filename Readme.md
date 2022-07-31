Ping all hosts

```
ansible selected -m ping
```

Get ip addresses

```
ansible selected -m debug -a msg="{{ ansible_default_ipv4.address|default(ansible_all_ipv4_addresses[0]) }}"
```