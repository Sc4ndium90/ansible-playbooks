## playbook-lxc-gpu-ollama.yml

Before running the playbook, the LXC container must be created as a Privileged system and nesting=1. The following lines must be added to the LXC conf file (check the path on Proxmox before).

```bash
lxc.cgroup2.devices.allow: c 226:1 rwm
lxc.cgroup2.devices.allow: c 226:128 rwm
lxc.mount.entry: /dev/dri/card1 dev/dri/card1 none bind,optional,create=file
lxc.mount.entry: /dev/dri/renderD128 dev/dri/renderD128 none bind,optional,create=file
```
