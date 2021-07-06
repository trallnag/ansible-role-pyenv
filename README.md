[![role](https://img.shields.io/ansible/role/54870)](https://galaxy.ansible.com/trallnag/pyenv)
[![quality](https://img.shields.io/ansible/quality/54870)](https://galaxy.ansible.com/trallnag/pyenv)
[![downloads](https://img.shields.io/ansible/role/d/54870?label=downloads)](https://galaxy.ansible.com/trallnag/pyenv)

# Ansible Role `pyenv`

Ansible role that installs pyenv on Ubuntu and Debian.

Available on [Ansible Galaxy](https://galaxy.ansible.com/trallnag/pyenv).

## Role Variables

None.

## Example Playbook

```yaml
- name: Playbook
  hosts: myhost
  remote_user: myuser
  vars:
    rolespec_validate: true
  roles:
    - name: trallnag.pyenv
```

## Special Requirements

None.

## Special Dependencies

None.

## License

Apache-2.0

## Author Information

Trallnag
