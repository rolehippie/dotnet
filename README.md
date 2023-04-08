# dotnet

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/dotnet)
[![General Workflow](https://github.com/rolehippie/dotnet/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/dotnet/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/dotnet/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/dotnet/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/dotnet/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/dotnet/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/dotnet)](https://github.com/rolehippie/dotnet/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.dotnet-blue)](https://galaxy.ansible.com/rolehippie/dotnet)

Ansible role to install .NET packages from Microsoft repos.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Default Variables](#default-variables)
  - [dotnet_packages](#dotnet_packages)
  - [dotnet_repo_distribution](#dotnet_repo_distribution)
  - [dotnet_repo_release](#dotnet_repo_release)
  - [dotnet_repo_version](#dotnet_repo_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### dotnet_packages

List of packages to install

#### Default value

```YAML
dotnet_packages:
  - dotnet-runtime-6.0
  - aspnetcore-runtime-6.0
```

### dotnet_repo_distribution

Enforce another distribution for the repo

#### Default value

```YAML
dotnet_repo_distribution: '{{ ansible_distribution | lower }}'
```

### dotnet_repo_release

Enforce another release for the repo

#### Default value

```YAML
dotnet_repo_release: '{{ ansible_distribution_release }}'
```

### dotnet_repo_version

Enforce another version for the repo

#### Default value

```YAML
dotnet_repo_version: '{{ ansible_distribution_version }}'
```

## Discovered Tags

**_dotnet_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
