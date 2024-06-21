# Ansible Role: GO

[![CI](https://github.com/trfore/ansible-role-go/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/trfore/ansible-role-go/actions/workflows/ci.yml)
[![CD](https://github.com/trfore/ansible-role-go/actions/workflows/cd.yml/badge.svg?branch=main)](https://github.com/trfore/ansible-role-go/actions/workflows/cd.yml)

Install Go Language

## Install the Role

You can install this role with the Ansible Galaxy CLI:

```bash
ansible-galaxy role install trfore.go
```

You can also include it in a `requirements.yml` file and install it with
`ansible-galaxy role install -r requirements.yml`, using the format:

```yaml
---
roles:
  - trfore.go
```

## Tested Platforms

- `ansible-core` 2.15, 2.16 & 2.17
- CentOS Stream 9
- Debian 12
- Ubuntu 22.04 & 24.04

## Role Variables

| Variable     | Default  | Description                                    | Required |
| ------------ | -------- | ---------------------------------------------- | -------- |
| `go_version` | `latest` | String, role will download the latest version. | No       |

## Example Playbook

```yaml
- hosts: servers
  gather_facts: true
  roles:
    - name: Install Go Lang
      role: trfore.go
```

## License

See [LICENSE](LICENSE) File

## Author Information

Taylor Fore (<https://github.com/trfore>)

## References

- <https://go.dev/doc/>
