## go

[![CI](https://github.com/Oefenweb/ansible-go/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-go/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-go-blue.svg)](https://galaxy.ansible.com/Oefenweb/go/)

Set up (the latest or a specific version of) [Go](https://golang.org/) in Debian-like systems.

#### Requirements

None

#### Variables

* `go_version`: [default: `go version go1.15 linux/amd64`]: Version string (to check)
* `go_tarball`: [default: `go1.15.linux-amd64.tar.gz`]: Tarball to install
* `go_tarball_checksum`: [default: `sha256:2d75848ac606061efe52a8068d0e647b35ce487a15bb52272c427df485193602`]: Tarball checksum (to check)

* `go_install_prefix`: [default: `/usr/local`]: Install prefix

* `go_remove_distro_version`: [default: `true`]: Whether or not to remove distribution versions

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - oefenweb.go
```

#### License

MIT

#### Author Information

Mischa ter Smitten (based on work of [Joshua Lund](https://github.com/jlund) and [Mahesh Paolini-Subramanya](https://github.com/dieswaytoofast))

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-go/issues)!
