# Ansible Role: WineHQ

Install WineHQ via PPA repository.

- Add GPG repository key
- Add WineHQ repository
- Enable i386 support if needed
- Install WineHQ
- Install PlayOnLinux (optional)
- Install Winetricks (optional)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

| Name           | Default Value   | Description                        |
| -------------- | --------------- | -----------------------------------|
| `winehq.install_playonlinux` | true | Whether to install PlayOnLinux |
| `winehq.install_winetricks` | true | Whether to install Winetricks |

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: all
  gather_facts: yes
  become: true

  roles:
    - role: jakoblichterfeld.winehq

```

## License

MIT

## Author Information

This role was created in 2023 by [Jakob Lichterfeld](https://github.com/JakobLichterfeld).
