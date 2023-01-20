# Ansible role Recover Consul Cluster

Ansible role to recover a Consul Cluster that is unable to elect a leader.

## Requirements

NONE

## Role Variables

| Variable Name   | Description           | Default     |
|-----------------|-----------------------|-------------|
| consul_data_dir | Consul data directory | /opt/consul |

## Dependencies

NONE

## Example Playbook

```yml
---
- name: Playbook to recover a Consul Cluster that has no leader
  hosts: consul
  gather_facts: yes

  roles:
    - ashleykleynhans.recover_consul_cluster
```

## License

GPLv3

## Author Information

Ashley Kleynhans
