[![role](https://img.shields.io/ansible/role/55570)](https://galaxy.ansible.com/trallnag/pyenv)
[![quality](https://img.shields.io/ansible/quality/55570)](https://galaxy.ansible.com/trallnag/pyenv)
[![downloads](https://img.shields.io/ansible/role/d/55570?label=downloads)](https://galaxy.ansible.com/trallnag/pyenv)

# Ansible Role `trallnag.pyenv`

Ansible role that installs [`pyenv`][pyenv] for Bash on Linux.

[pyenv]: https://github.com/pyenv/pyenv

Available on [Ansible Galaxy](https://galaxy.ansible.com/trallnag/pyenv).

## Content

* Installs all dependencies required by Pyenv.
* Installs Pyenv using the official installer.
* Adds init blocks to `.bashrc` and `.profile`.
* Installs `pyenv-virtualenv` plugin.
* Installs a global version of Python and enables it.

## Role Variables

```yaml
pyenv_global_python_version:
  default: 3.9.6
  type: raw
  required: false
  description: >-
    Poetry version to install and activate globally.
```

## Example Playbook

```yaml
- name: Playbook
  hosts: myhost
  remote_user: myuser
  vars:
    rolespec_validate: true
  roles:
    - name: trallnag.pyenv
      vars:
        pyenv_global_python_version: 3.9.6

pyenv_os_pkgs:
  default: []
  type: list
  elements: str
  required: false
  description: >-
    This role only installs the correct OS dependencies for the OS families
    Debian (for example Ubuntu) and RedHat (for example Fedora). If you
    are targeting another OS family you must list all required packages
    or a task in this role will fail.
```

## Special Requirements

None.

## Special Dependencies

None.

## License

Apache-2.0

## Author Information

Trallnag
