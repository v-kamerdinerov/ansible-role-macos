# v-kamerdinerov.macos

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/v-kamerdinerov/ansible-role-macos/CI?label=CI)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/v-kamerdinerov/ansible-role-macos/Release?label=Release)
![GitHub](https://img.shields.io/github/license/v-kamerdinerov/ansible-role-macos)
[![GitHub tag](https://img.shields.io/github/tag/v-kamerdinerov/ansible-role-macos.svg)](https://github.com/v-kamerdinerov/ansible-role-macos/tags)

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

## Author

Michael Savin aka `@jtprogru`

Twitter: [![Twitter Follow](https://img.shields.io/twitter/follow/jtprogru?color=gree&style=plastic)](https://twitter.com/jtprogru/)

## License

See [LICENSE](LICENSE)
