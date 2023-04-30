# v-kamerdinerov.macos

![GitHub CI Status](https://github.com/v-kamerdinerov/ansible-role-macos/actions/workflows/ci.yml/badge.svg)
![GitHub](https://img.shields.io/github/license/v-kamerdinerov/ansible-role-macos)  

This is simple ansible role for configure hostname and install my favorite soft from Homebrew and Mac App Store.


## Role Variables


See [`defaults/main.yml`](defaults/main.yml).


## Example Playbook

Example playbook:
```yaml
---
- name: macOS
  hosts: localhost
  connection: local
  become: false
  gather_facts: true

  vars:
    macos_hostname: "cronus"
    macos_homebrew_tap_ext:
      - coreutils
      - ghc

  roles:
    - v-kamerdinerov.macos
```


## License

See [LICENSE](LICENSE)
